<template>
  <div class="hello">
    <h2>YouTube</h2>

    <div class="player"></div>

    <div class="sub-list">
      <ul class="comp">
        <li>Luke Smith</li>
        <li>Hak5</li>
        <li>N-O-D-E</li>
      </ul>

      <ul class="ten">
        <li>David Dobrik</li>
        <li>Zane Hijazi</li>
        <li>Heath Hussar</li>
      </ul>

      <ul class="ent">
        <li>Sam & Niko</li>
        <li>Node</li>
        <li>Corridor</li>
        <li>Matt & Tom</li>
        <li>Modern Rouge</li>
        <li>Casey Neistat</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'YouTube',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h2 {
  margin-left: 3vw;
}

.player {
  background-color: #333;
  width: 70vw;
  height: 25vw;
  margin: 0 auto;
}

.sub-list {
  display: grid;
  grid-template-rows: 1fr;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  margin-left: 27vw;  

  li {
    width: 10vw;
    background-color: #333;
    margin: 10px 0;
    padding: 3px;
    border: 1px solid #00ff6c;
    border-radius: 3px;
    text-align: center;
  } 

  .comp {
    grid-column: 1/2;
    list-style: none;
  }

  .ten {
    grid-column: 2/3;
    list-style: none;
  }

  .ent {
    grid-column: 3/4;
    list-style: none;
  }
}
</style>
