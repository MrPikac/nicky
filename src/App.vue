<template>
  <div @click="something" id="app">
        <img id="nick" alt="Nicky" src="./assets/tumblr_mqg78sIALY1swnmv6o1_400.png">
  </div>
</template>

<script>

export default {
  name: 'app',
  components: {

  },
  data() {

  },

  methods: {
    something: function() {
      var x = event.clientX;
      var y = event.clientY;
      var img = document.getElementById("nick");
      img.style.left = this.x;
      img.style.top = this.y;
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
