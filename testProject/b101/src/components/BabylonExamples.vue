<template>
<div>
  <h3> Babylon Examples </h3>
  <canvas></canvas>
</div>
</template>

<script>
import { defineComponent } from 'vue';
import { BasicScene } from '@/BabylonExamples/BasicScenes';
export default defineComponent( {
  name: 'BabylonExamples',
  mounted(){
    const canvas = document.querySelector("canvas");
    new BasicScene(canvas);
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
