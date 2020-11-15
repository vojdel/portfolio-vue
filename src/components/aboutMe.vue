<template>
  <section class="container">
    <div class="row mt-5">
      <div class="col-6">
        <h4 class="text-center">Sobre Mi</h4><br>
        <p>Soy Desarrollador Web, soy amante de la musica, comics, mangas,
de los libros en general y autodidactad en programación.</p>
        <p>Me desempeño en las tecnologias como  javascript con Vue.js de
Front-end y Node.js de back-end, pero tambien PHP y Laravel</p>
      </div>
      <div class="col-6">
        <div class="card shadow p-3 mb-5 bg-white rounded">
          <div class="card-body">
            <p>
            <strong class="text-dark">Fecha de Nacimiento</strong>: {{ fdn }} <br><br>
            <strong>Lenguajes hablados</strong>: {{ allLenguages }}<br><br>
            <strong>Nacionalidad</strong>: {{ nacionalidad }}<br><br>
            <strong>Preferencias</strong>: {{ preferencs }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      fdn: "09-06-1999",
      languages: [
        'Español(materno)',
        'Inglés(Intermedio)'
             ],
      nacionalidad: 'Venezolano',
      preferencs: `Escuchar música (rock & metal) y Leer libros de ciencia
        ficcion, y aventuras`
    
    }
  },
  computed: {
    allLenguages: function(){
      return `${this.languages[0]}, ${this.languages[1]}`
    }
  }
}
</script>

<style>
</style>
