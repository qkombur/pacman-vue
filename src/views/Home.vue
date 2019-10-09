<template>
  <div class="home" v-on:keydown="inputHandler()">
    <Player 
    />
  </div>
</template>

<script>

import Player from '@/components/Player.vue'

export default {
  name: 'home',
  components: {
    Player
  }
  
}
</script>
