<script setup lang="ts">
  import Card from "./components/Card.vue";
  import ObjectCard from "./components/ObjectCard.vue";

  import CassettePlayer from "./assets/CassettePlayer.jpg";
  import DisposableCamera from "./assets/Disposable.jpg";
  import DSLRCamera from "./assets/DSLR.jpg";
  import FilmRoll from "./assets/Film.jpg";
  import FilmCamera from "./assets/FilmCam.jpg";
  import TelloDrone from "./assets/Tello.jpg";
</script>

<template>
  <div class="main">
    <Card style="width: fit-content; font-size: 16pt; text-align: center;">
      <h1 style="font-size: 54pt; font-weight: 200;">This website is not available at the moment.</h1>
      This website was created by infinity-atom.<br>
      Email domains.jameswhyyougottakeepbringingrandomstufftoschool.lol@infinity-atom.org for help, concerns, or questions. 
    </Card>
  </div>
</template>

<style scoped>
  .main {
    padding: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;

    box-sizing: border-box;
  }

  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    gap: 10px;

    margin-bottom: 10px;
  }
</style>