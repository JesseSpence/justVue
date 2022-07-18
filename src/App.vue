<template>
<Navbar />
  <router-view/>
</template>

<script>
import Navbar from "./components/Navbar.vue";

export default {
  components: {
    Navbar,
  },
};
</script>

<style>
:root {
    --highlight-color:#A71D31  /*crimson UA*/;
    --text-color:#F1F0CC;    /*light goldenrod yellow*/
    --background-color:#D5BF86; /*ecru beigh*/
    --el-color: #3F0D12; /*dark sienna*/
    --text-mute:#8D775F;
}

body {
color: var(--text-color)!important ;
background-color: var(--background-color) !important;
  background-color: rgb(0, 0, 0);
  
}
#app {
  
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2C3E50;
}
nav {
  padding: 30px;
}
</style>
