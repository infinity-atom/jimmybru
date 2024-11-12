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
    <Card style="text-align: center; margin-bottom: 10px;">
      <span style="font-size: 20pt; font-weight: bold;">James, why you gotta keep bringing random stuff to school?</span><br>
      <span style="font-size: 14pt">Don't you realize that what you're doing is really pointless?</span>
    </Card>
    <Card style="margin-bottom: 10px;">
      This is the stuff you've brought to school, for some reason.
    </Card>

    <div class="grid">
      <ObjectCard :img-url="CassettePlayer">
        Cassette Player
      </ObjectCard>
      <ObjectCard :img-url="DisposableCamera">
        Disposable Camera
      </ObjectCard>
      <ObjectCard :img-url="DSLRCamera">
        DSLR Camera
      </ObjectCard>
      <ObjectCard :img-url="FilmCamera">
        Film Camera <small>(x2)</small>
      </ObjectCard>
      <ObjectCard :img-url="FilmRoll">
        5mm Film Roll
      </ObjectCard>
      <ObjectCard :img-url="TelloDrone">
        Tello Drone
      </ObjectCard>
    </div>

    <Card>
      This website was created by <a style="color: white;" href="https://infinity-atom.org">infinity-atom</a>.<br>
      Email <a style="color: white;" href="mailto:domains.jameswhyyougottakeepbringingrandomstufftoschool.lol@infinity-atom.org">domains.jameswhyyougottakeepbringingrandomstufftoschool.lol@infinity-atom.org</a> for help, concerns, or questions.
    </Card>
  </div>
</template>

<style scoped>
  .main {
    padding: 10px;
  }

  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    gap: 10px;

    margin-bottom: 10px;
  }
</style>