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
      <div class="row">
        <div class="col">
          Par
        </div>
        <div class="col">
          {{hole1Par}}
        </div>
        <div class="col">
          {{hole2Par}}
        </div>
        <div class="col">
          {{hole3Par}}
        </div>
        <div class="col">
          {{hole4Par}}
        </div>
        <div class="col">
          {{hole5Par}}
        </div>
        <div class="col">
          {{hole6Par}}
        </div>
        <div class="col">
          {{hole7Par}}
        </div>
        <div class="col">
          {{hole8Par}}
        </div>
        <div class="col">
          {{hole9Par}}
        </div>
        <div class="col">
          {{frontsidePar}}
        </div>
        <div class="col">
          {{hole10Par}}
        </div>
        <div class="col">
          {{hole11Par}}
        </div>
        <div class="col">
          {{hole12Par}}
        </div>
        <div class="col">
          {{hole13Par}}
        </div>
        <div class="col">
          {{hole14Par}}
        </div>
        <div class="col">
          {{hole15Par}}
        </div>
        <div class="col">
          {{hole16Par}}
        </div>
        <div class="col">
          {{hole17Par}}
        </div>
        <div class="col">
          {{hole1Par}}
        </div>
         <div class="col">
          {{backsidePar}}
        </div>
         <div class="col">
          {{totalPar}}
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