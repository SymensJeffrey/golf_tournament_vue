<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div class="container">
      <div class="row">
        <div class="col">
          {{golfCourseName}}
        </div>
      </div>
      <div class="row">
        <div class="col">
          Hole
        </div>
        <div class="col">
          1
        </div>
        <div class="col">
          2
        </div>
        <div class="col">
          3
        </div>
        <div class="col">
          4
        </div>
        <div class="col">
          5
        </div>
        <div class="col">
          6
        </div>
        <div class="col">
          7
        </div>
        <div class="col">
          8
        </div>
        <div class="col">
          9
        </div>
        <div class="col">
          Out
        </div>
        <div class="col">
          10
        </div>
        <div class="col">
          11
        </div>
        <div class="col">
          12
        </div>
        <div class="col">
          13
        </div>
        <div class="col">
          14
        </div>
        <div class="col">
          15
        </div>
        <div class="col">
          16
        </div>
        <div class="col">
          17
        </div>
        <div class="col">
          18
        </div>
         <div class="col">
          In
        </div>
         <div class="col">
          Total
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.col{
  border-style: solid;
  border-width: 1px;
}
</style>

<script>
  export default {
    data: function () {
      return {
        message: "Welcome to the 2022 Symens Open",
        golfCourseName: "Pebble Beach"
      };
    },
    created: function () {},
    methods: {},
  };
</script>