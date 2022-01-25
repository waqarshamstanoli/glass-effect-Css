<template>
  <v-container class="body">

<div class="glass">
</div>
  </v-container>
</template>
<script>

export default {
  data() {
    return {

       
    };
  },

  

};
</script>

<style scoped>
.body {
  background: url('https://ichef.bbci.co.uk/news/976/cpsprodpb/6C55/production/_120433772_gettyimages-945627318.jpg') no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.glass {
  position: relative;
  background: inherit;
  overflow: hidden;
  width: 50%;
  height: 50%;
  border-radius: 1px;
  box-shadow: 0 6px 0px rgba(0, 0, 0, 0.1), 
              0 6px 0px rgba(0, 0, 0, 0.1);
  z-index: 1;
}

.glass:before {
  content: '';
  position: absolute;
  background: inherit;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  margin: -20px;
  box-shadow: inset 0 0 500px rgba(255, 255, 255, .4); 
  filter: blur(10px);
  z-index: -1;
}
</style>
