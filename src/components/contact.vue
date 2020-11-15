<template>
  <section class="container">
    <div class="row">
      <diV class="col-5">
        <h4 class="text-center">Contáctame</h4><br>
          <div class="contact-info row">
            <div class="col-2"><i class="fas fa-phone"></i></div>
            <div class="col-10"><h5>Telefono:</h5>
            <span>{{ tlf.region }}{{ tlf.numero }}</span></div>
          </div>
          <div class="contact-info row">
            <div class="col-2"><i class="fas fa-envelope"></i></div>
            <div class="col-10"><h5>Correo:</h5>
            {{ email }}</div>
          </div> 
          <div class="contact-info row">
            <div class="col-2"><i class="fas
fa-map-marker-alt"></i></div>
            <div class="col-10"><h5>Dirrección:</h5>
            {{ address }}</div>
          </div> 
      </div>
      <div class="col-7">
        <div class="card">
          <form action="#">
            <div class="car-title"><h3 class="text-center">Enviame un Mensaje</h3></div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      tlf: { region: "(+58)", numero: "0424-5879762" },
      email: "vasquezpinedaj@gmail.com",
      address: `calle el galpon, frente al mercal, Sabana Larga, Yaracuy, Venezuela.`
    }
  }
}
</script>

<style scope>
  .contact-info{
     margin-bottom: 20px;
  }

  .contact-info i{
    color: #044790c2;
    font-size: 40px;
  }
</style>
