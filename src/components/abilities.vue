<template>
  <section class="container p-4">
    <div class="row">
      <div class="col"><h4 class="text-center">Habilidades</h4></div>
    </div>
    <div class="row">
      <div class="col">
        <div class="row" v-for="item in abilities" :key="item.id">
          <strong class="col">{{ item.abilitie }}</strong><span class="col
text-right">{{ item.value }}%</span><br>
          <progress max="100" :value="item.value" class="w-100">{{
item.value }}%</progress><br>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      abilities: [
        { abilitie: 'HTML5 | CSS3', value: 80 },
        { abilitie: 'Javascript | Vuejs', value: 85 },
        { abilitie: 'Nodejs', value: 75 },
        { abilitie: 'PHP | Laravel', value: 80 },
        { abilitie: 'Mysql | Postgresql', value: 65 },
        { abilitie: 'Python', value: 30 },
        { abilitie: 'Git | Github', value: 75 },
      ]
    }
  }
}
</script>

<style scope>
  progress{
      height: 22.5px;
  }
</style>
