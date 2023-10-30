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
    <section class="container text-center mb-5 pb-5">
    <div class="div gif-pc-cont">
      <img src="../assets/pc.png" alt="" class="gif-pc">
    </div>
      <FuchsiaButton :buttonText="'Quiero mi landing page'" class="my-4"/>
      <h2 class="">Comunica el mensaje de tu <span class="purple-text">negocio, servicio o lanzamiento</span></h2>
      <p class="grey-text">de una manera directa y captando la atención de tu cliente objetivo con un <span class="bold-text">atractivo landing page</span>.</p>
    </section>
    <WaveComp class="invertir"/>
    <section id="incluye" class="text-center">
      <div class="container">
        <h2 class="pink-text">¿Qué incluye?</h2>
        <p class="white-text">Diseño y desarrollo de un landing page incluyendo 6 secciones:</p>
        <div class="secciones">
          <div class="seccion-left">
            <p>Header + Llamado a la acción</p>
          </div>
          <div class="seccion seccion-right">
            <p>Propuesta de valor</p>
          </div>
          <div class="seccion-left">
            <p>Beneficios / Valor agregado</p>
          </div>
          <div class="seccion seccion-right">
            <p>Referencias / Testimonios</p>
          </div>
          <div class="seccion-left">
            <p>Datos de contacto + Formulario</p>
          </div>
          <div class="seccion seccion-right">
            <p>Preguntas frecuentes</p>
          </div>
          <div class="seccion-left bg-pink">
            <p>Pixel de facebook y Google Analytics</p>
          </div>
           <div class="seccion-right bg-pink">
            <p>Whatsapp visible en toda la web</p>
          </div>
        </div>
        <p class="white-text">Precio lanzamiento: <span class="pink-text big-text">$159.000 +iva </span><span class="tachado">$257.000 + iva</span></p>
        <FuchsiaButton :buttonText="'Quiero mi landing page'" class="my-4"/>
        <p class="little-text white-text">¡Solo 10 cupos a este precio!</p>
        <p class="little-text white-text pt-5">*El precio no incluye dominio y hosting, debes tenerlo tu. Pero no te preocupes que si no sabes de ello te contamos como hacerlo. <br>*Cualquier sección adicional tendrá un costo asociado que debemos cotizar en caso de ser requerida.</p>
      </div>
    </section>
    <PinkWave/>
  </div>
</template>

<script>
// @ is an alias to /src
import PreHeader from '@/components/PreHeader.vue'
import FuchsiaButton from '@/components/FuchsiaButton.vue'
import WaveComp from '@/components/WaveComp.vue'
import PinkWave from '@/components/PinkWave.vue'

export default {
  name: 'HomeView',
  components: {
    PreHeader,
    FuchsiaButton,
    WaveComp,
    PinkWave
  }
}
</script>
