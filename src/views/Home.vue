<template>
  <div class="home">
    <h1 class="title-center-text">{{ message }}</h1>
    <div class="container">
      <div class="row">
      </div>
      <!-- Holes -->
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
      <!-- Par -->
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
      <!-- Player 1 -->
      <div v-for="player1 in player1s">
        <div class="row">
          <div class="col">
            Player 1
          </div>
          <div class="col">
            {{player1.hole1}}
          </div>
          <div class="col">
            {{player1.hole2}}
          </div>
          <div class="col">
            {{player1.hole3}}
          </div>
          <div class="col">
            {{player1.hole4}}
          </div>
          <div class="col">
            {{player1.hole5}}
          </div>
          <div class="col">
            {{player1.hole6}}
          </div>
          <div class="col">
            {{player1.hole7}}
          </div>
          <div class="col">
            {{player1.hole8}}
          </div>
          <div class="col">
            {{player1.hole9}}
          </div>
          <div class="col">
            {{player1Front}}
          </div>
          <div class="col">
            {{player1.hole10}}
          </div>
          <div class="col">
            {{player1.hole11}}
          </div>
          <div class="col">
            {{player1.hole12}}
          </div>
          <div class="col">
            {{player1.hole13}}
          </div>
          <div class="col">
            {{player1.hole14}}
          </div>
          <div class="col">
            {{player1.hole15}}
          </div>
          <div class="col">
            {{player1.hole16}}
          </div>
          <div class="col">
            {{player1.hole17}}
          </div>
          <div class="col">
            {{player1.hole18}}
          </div>
          <div class="col">
            {{player1Back}}
          </div>
          <div class="col">
            {{totalPar}}
          </div>
        </div>
      </div>
      <!-- Player 2 -->
      <div v-for="player2 in player2s">
        <div class="row">
          <div class="col">
            Player 2
          </div>
          <div class="col">
            {{player2.hole1}}
          </div>
          <div class="col">
            {{player2.hole2}}
          </div>
          <div class="col">
            {{player2.hole3}}
          </div>
          <div class="col">
            {{player2.hole4}}
          </div>
          <div class="col">
            {{player2.hole5}}
          </div>
          <div class="col">
            {{player2.hole6}}
          </div>
          <div class="col">
            {{player2.hole7}}
          </div>
          <div class="col">
            {{player2.hole8}}
          </div>
          <div class="col">
            {{player2.hole9}}
          </div>
          <div class="col">
            {{frontsidePar}}
          </div>
          <div class="col">
            {{player2.hole10}}
          </div>
          <div class="col">
            {{player2.hole11}}
          </div>
          <div class="col">
            {{player2.hole12}}
          </div>
          <div class="col">
            {{player2.hole13}}
          </div>
          <div class="col">
            {{player2.hole14}}
          </div>
          <div class="col">
            {{player2.hole15}}
          </div>
          <div class="col">
            {{player2.hole16}}
          </div>
          <div class="col">
            {{player2.hole17}}
          </div>
          <div class="col">
            {{player2.hole18}}
          </div>
          <div class="col">
            {{backsidePar}}
          </div>
          <div class="col">
            {{totalPar}}
          </div>
        </div>
      </div>
      <!-- Player 3 -->
      <div v-for="player3 in player3s">
        <div class="row">
          <div class="col">
            Player 3
          </div>
          <div class="col">
            {{player3.hole1}}
          </div>
          <div class="col">
            {{player3.hole2}}
          </div>
          <div class="col">
            {{player3.hole3}}
          </div>
          <div class="col">
            {{player3.hole4}}
          </div>
          <div class="col">
            {{player3.hole5}}
          </div>
          <div class="col">
            {{player3.hole6}}
          </div>
          <div class="col">
            {{player3.hole7}}
          </div>
          <div class="col">
            {{player3.hole8}}
          </div>
          <div class="col">
            {{player3.hole9}}
          </div>
          <div class="col">
            {{frontsidePar}}
          </div>
          <div class="col">
            {{player3.hole10}}
          </div>
          <div class="col">
            {{player3.hole11}}
          </div>
          <div class="col">
            {{player3.hole12}}
          </div>
          <div class="col">
            {{player3.hole13}}
          </div>
          <div class="col">
            {{player3.hole14}}
          </div>
          <div class="col">
            {{player3.hole15}}
          </div>
          <div class="col">
            {{player3.hole16}}
          </div>
          <div class="col">
            {{player3.hole17}}
          </div>
          <div class="col">
            {{player3.hole18}}
          </div>
          <div class="col">
            {{backsidePar}}
          </div>
          <div class="col">
            {{totalPar}}
          </div>
        </div>
      </div>
      <!-- Player 4 -->
      <div v-for="player4 in player4s">
        <div class="row">
          <div class="col">
            Player 4
          </div>
          <div class="col">
            {{player4.hole1}}
          </div>
          <div class="col">
            {{player4.hole2}}
          </div>
          <div class="col">
            {{player4.hole3}}
          </div>
          <div class="col">
            {{player4.hole4}}
          </div>
          <div class="col">
            {{player4.hole5}}
          </div>
          <div class="col">
            {{player4.hole6}}
          </div>
          <div class="col">
            {{player4.hole7}}
          </div>
          <div class="col">
            {{player4.hole8}}
          </div>
          <div class="col">
            {{player4.hole9}}
          </div>
          <div class="col">
            {{frontsidePar}}
          </div>
          <div class="col">
            {{player4.hole10}}
          </div>
          <div class="col">
            {{player4.hole11}}
          </div>
          <div class="col">
            {{player4.hole12}}
          </div>
          <div class="col">
            {{player4.hole13}}
          </div>
          <div class="col">
            {{player4.hole14}}
          </div>
          <div class="col">
            {{player4.hole15}}
          </div>
          <div class="col">
            {{player4.hole16}}
          </div>
          <div class="col">
            {{player4.hole17}}
          </div>
          <div class="col">
            {{player4.hole18}}
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
  </div>
</template>

<style>
.col{
  min-width: 30px;
  border-style: solid;
  border-width: 1px;
}
.row{
  text-align: center;
  min-width: 1200px;
  resize: none;
  overflow: scroll;
}
.title-center-text{
  text-align: center;
  padding-bottom: 15px;
}
</style>

<script>
  import axios from 'axios'
  export default {
    data: function () {
      return {
        message: "Welcome to Golf Tracker",
        hole1Par: 4,
        hole2Par: 4,
        hole3Par: 4,
        hole4Par: 4,
        hole5Par: 4,
        hole6Par: 4,
        hole7Par: 4,
        hole8Par: 4,
        hole9Par: 4,
        hole10Par: 4,
        hole11Par: 4,
        hole12Par: 4,
        hole13Par: 4,
        hole14Par: 4,
        hole15Par: 4,
        hole16Par: 4,
        hole17Par: 4,
        hole18Par: 4,
        frontsidePar: 0,
        backsidePar: 0,
        totalPar: 0,
        player1s: [],
        player1Front: 0,
        player1Back: 0,
        player2s: [],
        player3s: [],
        player4s: [],
      };
    },
    created: function () {
      this.frontsideParCalc();
      this.backsideParCalc();
      this.totalParCalc();
      this.player1Index();
      this.player2Index();
      this.player3Index();
      this.player4Index();
    },
    methods: {
      frontsideParCalc: function() {
        this.frontsidePar = this.hole1Par + this.hole2Par + this.hole3Par + this.hole4Par + this.hole5Par + this.hole6Par + this.hole7Par + this.hole8Par + this.hole9Par
      },
      backsideParCalc: function() {
        this.backsidePar = this.hole10Par + this.hole11Par + this.hole12Par + this.hole13Par + this.hole14Par + this.hole15Par + this.hole16Par + this.hole17Par + this.hole18Par
      },
      totalParCalc: function() {
        this.totalPar = this.frontsidePar + this.backsidePar
      },
      player1Index: function() {
        axios.get("/player1s").then((response) => {
          console.log("player 1 index", response);
          this.player1s = response.data
          this.player1Front = response.data[0].hole1 + response.data[0].hole2 + response.data[0].hole3 + response.data[0].hole4 + response.data[0].hole5 + response.data[0].hole6 + response.data[0].hole7 + response.data[0].hole8 + response.data[0].hole9
          this.player1Back = response.data[0].hole10 + response.data[0].hole11 + response.data[0].hole12 + response.data[0].hole13 + response.data[0].hole14 + response.data[0].hole15 + response.data[0].hole16 + response.data[0].hole17 + response.data[0].hole18
        })
      },
      player2Index: function() {
        axios.get("/player2s").then((response) => {
          console.log("player 2 index", response);
          this.player2s = response.data
        })
      },
      player3Index: function() {
        axios.get("/player3s").then((response) => {
          console.log("player 3 index", response);
          this.player3s = response.data
        })
      },
      player4Index: function() {
        axios.get("/player4s").then((response) => {
          console.log("player 4 index", response);
          this.player4s = response.data
        })
      },
    },
  };
</script>