<template>
  <div id="app">
    <nav>
      <span class="relax active"> Relax </span>
      <span class="work inactive"> Work </span>
      <span class="line"></span>
    </nav>

    <YouTube></YouTube>
    <Messenger></Messenger>
    <Facebook></Facebook>
  </div>
</template>

<script>
import YouTube from './components/Youtube'
import Messenger from './components/Messenger'
import Facebook from './components/Facebook'

export default {
  name: 'app',
  components: {
    YouTube,
    Messenger,
    Facebook
  }
}
</script>

<style lang="scss">
#app {
  height: 100%;
  background-color: #1c1c1c;
  color: #fff;
  border: 3px solid #00ff6c;
  font-family: 'Fira Mono', monospace;

  a {
    color: inherit;
    text-decoration: none;
  }
}

nav {
  border-bottom: 3px solid #00ff6c;

  .active {
    z-index: 2;
    background-color: #1c1c1c;
    padding: 0 3vw 3vh 3vw;
  }
  .inactive {
    z-index: 1;
    padding: 0vh 3vw;
    border: 3px solid #00ff6c;
  }

  .line {
    border-right: 3px solid #00ff6c;
  }
}

</style>
