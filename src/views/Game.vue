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
  data () {
    return {
      games: ['Dota', 'CSGO']
    }
  }
};
</script>
