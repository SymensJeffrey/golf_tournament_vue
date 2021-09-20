<template>
  <div class="login">
      <div class="container-fluid ps-md-0">
        <div class="row g-0">
          <div class="d-none d-md-flex col-md-4 col-lg-6 bg-image"></div>
          <div class="col-md-8 col-lg-6">
            <div class="login d-flex align-items-center py-5">
              <div class="container">
                <div class="row">
                  <div class="col-md-9 col-lg-8 mx-auto">
                    <h3 class="login-heading mb-4">Welcome back!</h3>
                    <!-- Sign In Form -->
                    <form v-on:submit.prevent="submit()">
                      <ul>
                        <li v-for="error in errors" v-bind:key="error">{{ error }}</li>
                      </ul>
                      <div class="form-floating mb-3">
                        <input v-model="newSessionParams.email" type="email" class="form-control" id="floatingInput" placeholder="name@example.com">
                        <label for="floatingInput">Email address</label>
                      </div>
                      <div class="form-floating mb-3">
                        <input v-model="newSessionParams.password" type="password" class="form-control" id="floatingPassword" placeholder="Password">
                        <label for="floatingPassword">Password</label>
                      </div>
                      <div class="d-grid">
                        <button class="green-button btn btn-lg btn-primary btn-login text-uppercase fw-bold mb-2" type="submit">Sign in</button>
                      </div>
                    </form>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<style>
  .login {
    min-height: 100vh;
    width: 100%;
  }

  .bg-image {
    background-image: url('https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/64a1aa92-f4a6-4a1d-b8e1-6d04554f55fa/d8594wj-e2e66265-a7d3-44b5-9854-67bff5d6e376.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcLzY0YTFhYTkyLWY0YTYtNGExZC1iOGUxLTZkMDQ1NTRmNTVmYVwvZDg1OTR3ai1lMmU2NjI2NS1hN2QzLTQ0YjUtOTg1NC02N2JmZjVkNmUzNzYucG5nIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.gsSotNTlQA9jeNlDU1BK-Q4qnnkzNy0PQTqhY3Xg-l4');
    background-size: cover;
    background-position: center;
  }

  .login-heading {
    font-weight: 300;
  }

  .btn-login {
    font-size: 0.9rem;
    letter-spacing: 0.05rem;
    padding: 0.75rem 1rem;
  }

  .green-button{
    background-color: rgb(45, 187, 32);
    border: none;
  }
  .green-button:hover{
    background-color: rgb(115, 214, 106);
  }
</style>

<script>
  import axios from "axios";

  export default {
    data: function () {
      return {
        newSessionParams: {},
        errors: [],
      };
    },
    methods: {
      submit: function () {
        axios
          .post("/sessions", this.newSessionParams)
          .then((response) => {
            axios.defaults.headers.common["Authorization"] = "Bearer " + response.data.jwt;
            localStorage.setItem("jwt", response.data.jwt);
            this.$router.push("/");
          })
          .catch((error) => {
            console.log(error.response);
            this.errors = ["Invalid email or password."];
            this.email = "";
            this.password = "";
          });
      },
    },
  };
</script>
