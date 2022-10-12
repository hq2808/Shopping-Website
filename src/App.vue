<template>
 <div>
    <Navbar @toggle="toggleCart" />
 </div>
</template>
<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Navbar from "@/components/Navbar.vue";

@Component({
  components: {
    Navbar,
  },
})
export default class App extends Vue {}
</script>
<style>
@font-face {
  font-family: ITC Cheltenham Std;
  src: url(./fonts/CheltenhamStd.otf);
}
@font-face {
  font-family: Clab Personal Use;
  src: url(./fonts/ClabPersonalUse.otf);
}
@font-face {
  font-family: Magisho;
  src: url(./fonts/Magisho.otf);
}
@font-face {
  font-family: Hjet;
  src: url(./fonts/Hjet.otf);
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
  width: 100%;
  margin: 0;
  padding: 0;
  height: 100%;
}
.opacity {
  opacity: 0.8;
}

html,
body,
p,
h1,
h3 {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

textarea:focus,
input:focus {
  outline: none;
}

button:focus {
  outline: 0;
}

button {
  cursor: pointer;
}

img {
  user-select: none;
  -moz-user-select: none;
  -webkit-user-drag: none;
  -webkit-user-select: none;
  -ms-user-select: none;
}
</style>
