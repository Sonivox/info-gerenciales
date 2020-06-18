<template>
  <div class="">
    <div>
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <!-- LOGO -->
        <div class="logo text-center">
          <img src="./assets/DineroLogo.png" height="50" width="50"/>
          <h4>Outsourcing</h4>
        </div>

        <!-- MENU PANTALLA TELEFONOS -->
        <b-navbar-toggle target="nav-collapse"><b-icon icon="list-ul"></b-icon> Menu</b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav class="text-center">
          <!-- VUE ROUTERS -->
          <b-navbar-brand class="router" >
            <router-link style="text-decoration: none" to="/">Home</router-link>
          </b-navbar-brand>

          <b-navbar-nav class="router">
            <b-navbar-brand>
              <router-link style="text-decoration: none" to="/Planes">Planes</router-link>
            </b-navbar-brand>

            <b-navbar-brand>
              <router-link style="text-decoration: none" to="/sistemas">Sistemas</router-link>
            </b-navbar-brand>

            <b-navbar-brand>
              <router-link style="text-decoration: none" to="/contacto">Contactanos</router-link>
            </b-navbar-brand>

            <b-navbar-brand>
              <router-link style="text-decoration: none" to="/about">Nosotros</router-link>
            </b-navbar-brand>

          </b-navbar-nav>

          <!-- PARA EL USUARIO -->
          <b-navbar-nav class="ml-auto">
            <!-- SI NO ESTA LOGUEADO -->
            <div>

            </div>
            <!-- SI ESTA LOGUEADO -->
            <div>
              <b-dropdown id="dropdown-right" right variant="success" class="m-2">
                <template v-slot:button-content>
                  <b-icon icon="person-circle"></b-icon> Usuario
                </template>
                <b-dropdown-item href="#"><b-icon icon="info-circle"></b-icon>
                  Información</b-dropdown-item>
                <b-dropdown-divider></b-dropdown-divider>
                <b-dropdown-item href="#"><b-icon icon="power"></b-icon>
                  Cerrar sesión</b-dropdown-item>
                <b-dropdown-divider></b-dropdown-divider>
                <b-dropdown-item href="#" disabled><b-icon icon="alarm"></b-icon>
                  Futuro...</b-dropdown-item>
              </b-dropdown>
            </div>

          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <router-view/>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        user: 'Roberto'
      }
    }
  }
</script>

<style>
  .logo{
    padding: 0px 40px 0px 0px;
    color: white;
    font-family: 'Open Sans', sans-serif;
  }
  .router{
    text-decoration: none;
    font-weight: bold;
  }
  .router a{
    color: white;
  }
  .router a:hover{
    color: #5CF09B;
  }
  .router a.router-link-exact-active {
    color: #42b983;
  }
</style>
