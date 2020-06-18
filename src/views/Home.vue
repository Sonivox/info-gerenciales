<template>
  <div class="">

    <div class="titulo hero-image">
      <h1>Outsurcing</h1>
      <b-icon style="width: 120px; height: 120px; color: white" icon="code-slash"></b-icon>
      <div>
        <div>
          <h3>Tu mejor opción tecnológica para tu empresa.</h3>
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-sm-1"></div>
      <div class="col-sm-4 cover">
        <h3 class="text-center">Caracterizados por <b-icon icon="arrow-down-circle-fill"></b-icon></h3>
        <div style="padding: 0rem 1rem;">
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Datos confidenciales</h5>
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Aplicación segura</h5>
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Desarrollado a tu medida</h5>
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Interfaz amigable</h5>
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Control masivo de datos</h5>
          <h5><b-icon variant="success" icon="check2-circle"></b-icon> Pago automatico</h5>
        </div>
      </div>
      <div class="col-sm-2"></div>
      <div class="col-sm-4 text-center cover">
        <h3 class="text-center">Siempre disponibles <b-icon icon="emoji-sunglasses"></b-icon></h3><br>
        <h5>Siempre te podemos ayudar, solo sigue este enlace</h5><br>
        <b-button size="lg" pill variant="danger"><b-icon icon="headphones"></b-icon> Soporte remoto online</b-button>
      </div>
      <div class="col-sm-1"></div>
    </div>

    <div class="bg-light text-center">
      <h3 style="padding: 10px 0rem">Grandes y pequeñas empresas estan haciendo grandes cosas con nosotros.</h3>

      <div class="col">
        <b-card-group deck class="empresas">
          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>

          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>

          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>
        </b-card-group>

        <b-card-group deck class="empresas">
          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>

          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>

          <b-card img-src="https://placekitten.com/1000/500" img-alt="Card image" img-top>
            <b-card-text>
              Some quick example text to build on the card and make up the bulk of the card's content.
            </b-card-text>
          </b-card>
        </b-card-group>
      </div>
    </div>

    <Footer/>

  </div>
</template>

<script>
  import Footer from "@/components/Footer";
  export default {
    name: 'Home',
    props:{},
    components: {
      Footer
    }
}
</script>

<style>
  .titulo{
    text-align: center;
    font-family: 'Open Sans', sans-serif;
  }
  .titulo h1{
    font-size:50px;
    color: #3CE937;
  }
  .titulo h3{
    font-size:30px;
    font-weight: bold;
    color: white;
  }
  .hero-image {
    background-image: url("../assets/portada.jpg");
    background-color: #cccccc;
    height: 300px;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
  }
  .col{
    margin-right: 0px;
  }
  .empresas{
    padding: 2rem 0rem;
  }

</style>