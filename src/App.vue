<template>
  <div>
  <navegacion></navegacion>
  <h1>{{ tittle }}</h1>
  </div>
</template>

<script>
import Menu from './components/menu'
export default {
  components: {
    navegacion: Menu
            },
  data() {
    return {
    tittle: 'Welcome my Personal Page!!'
    }
  }
}
</script>

<style>
</style>
