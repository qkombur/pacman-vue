<template>
  <div>
    <svg
      xmlns="http://www.w3.org/2000/svg" 
      height="571.11" width="541.6">
      <path id=""d="M535.441 412.339a280.868 280.868 0 11.745-250.606L284.493 286.29z" fill="#fc0"/>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'Player',
  props: ['xPosition, yPosition'],
   data: function() {
    return {
      xPosition: 0,
      yPosition: 0
    }
  },

  methods: {

  },

  mounted: function() {
      window.addEventListener('keydown', event => {
        switch (event.key){
          case "ArrowLeft":
            console.log('left');
            this.xPosition += 1
            break;
          case "ArrowRight":
            console.log('right');
            break;
          case "ArrowUp":
            console.log('up');
            break;
          case "ArrowDown":
            console.log('down');
            break;
        }

      })
  }
}
</script>


<style scoped lang="scss">

</style>
