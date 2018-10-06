<template>
  <div class="home">
    <h1 class="terminal">
      {{ this.games[Math.floor(Math.random() * 2)] }}
    </h1>
  </div>
</template>

<script>
export default {
  name: "game",
  data() {
    return {
      games: ["Dota 2", "CSGO"]
    };
  }
};
</script>

<style scoped lang="scss">
div {
  display: inline-block;
  top: 50%;
  left: 50%;
  position: absolute;
  transform: translate(-51%, -50%);

  h1 {
    font-size: 8em;
    font-family: "Source Code Pro", monospace;
    font-weight: normal;
  }
}
</style>
