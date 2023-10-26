<template>
  <div class="home">
    <PreHeader/>
    <header>
      <nav class="container ml-auto">
        <img src="../assets/logo_vanilla_navbar.png" alt="">
        <FuchsiaButton :buttonText="'¡lo necesito!'"/>      
      </nav>
      <div class="container text-center main-title">
         <h1 class="white-text mb-4">¿Estás lista para lanzar tu servicio y <span class="pink-text">captar la atención</span>  de tus potenciales clientes?</h1>
         <p class="bajada">Tu negocio merece un landingpage que refleje lo <span class="bold-text">genial que es</span>.</p>
      </div>
    </header>
    <WaveComp/>
  </div>
</template>

<script>
// @ is an alias to /src
import PreHeader from '@/components/PreHeader.vue'
import FuchsiaButton from '@/components/FuchsiaButton.vue'
import WaveComp from '@/components/WaveComp.vue'

export default {
  name: 'HomeView',
  components: {
    PreHeader,
    FuchsiaButton,
    WaveComp
  }
}
</script>
