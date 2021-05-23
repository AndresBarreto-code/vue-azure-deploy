<template>
  <div id="app">
    <div id="nav">
      <router-link :to="{ name: 'Home' }">Home</router-link> |
      <router-link :to="{ name: 'About' }">About</router-link> |
      <router-link :to="{ name: 'Page1' }">Page 1</router-link> |
      <router-link :to="{ name: 'Page2' }">Page 2</router-link> |
      <router-link :to="{ name: 'Page3' }">Page 3</router-link> 
    </div>
    <router-view/>
  </div>
</template>
<script>

export default ({
  
})
</script>

<style lang="scss">
</style>
