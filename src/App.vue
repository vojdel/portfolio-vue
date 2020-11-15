<template>
  <div>
    <navegacion></navegacion>
    <aboutMe></aboutMe>
    <hr class="bg-seccondary w-100">
    <abilities></abilities>
    <hr class="bg-seccondary w-100">
    <contact></contact>
  </div>
</template>

<script>
import Menu from './components/menu'
import AboutMe from './components/aboutMe'
import Abilities from './components/abilities'
import Contact from './components/contact'

export default {
  components: {
    navegacion: Menu,
    aboutMe: AboutMe,
    abilities: Abilities,
    contact: Contact
            },
  data() {
    return {
    tittle: 'Welcome my Personal Page!!'
    }
  }
}
</script>

<style>
  h4{
      text-decoration: underline;
  }
</style>
