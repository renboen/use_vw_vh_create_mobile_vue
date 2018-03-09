<template>
  <div id="app">
    <h1>main</h1>
    <div class="title">uuu</div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  methods:{}
}
</script>

<style>
*{
  margin: 0;padding: 0;
}
:root{
  --cp:blue;
}
  :global .title {
 font-size: 100px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: var(--cp)
}
</style>
