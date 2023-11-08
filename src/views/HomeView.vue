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
         <p class="bajada">Tu negocio merece un landing page que refleje lo <span class="bold-text">genial que es</span>.</p>
      </div>
    </header>
    <WaveComp/>
    <section class="container text-center mb-5 pb-5" id="propuesta">
      <div class="div gif-pc-cont">
        <img src="../assets/animacion-landings.gif" alt="" class="gif-pc img-fluid">
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
            <p class="mini-little-p">Header + Llamado a la acción</p>
          </div>
          <div class="seccion seccion-right">
            <p class="mini-little-p">Propuesta de valor</p>
          </div>
          <div class="seccion-left">
            <p class="mini-little-p">Beneficios / Valor agregado</p>
          </div>
          <div class="seccion seccion-right">
            <p class="mini-little-p">Referencias / Testimonios</p>
          </div>
          <div class="seccion-left">
            <p class="mini-little-p">Datos de contacto + Formulario</p>
          </div>
          <div class="seccion seccion-right">
            <p class="mini-little-p">Preguntas frecuentes</p>
          </div>
          <div class="seccion-left bg-pink">
            <p class="mini-little-p">Pixel de facebook y Google Analytics</p>
          </div>
           <div class="seccion-right bg-pink">
            <p class="mini-little-p">Whatsapp visible en toda la web</p>
          </div>
        </div>
        <p class="white-text">Precio lanzamiento: <span class="pink-text big-text">$167.000 +iva </span><span class="tachado">$257.000 + iva</span></p>
        <FuchsiaButton :buttonText="'Quiero mi landing page'" class="my-4"/>
        <p class="little-text white-text">¡Solo 10 cupos a este precio!</p>
        <p class="little-text white-text pt-5">*El precio no incluye dominio y hosting, debes tenerlo tu. Pero no te preocupes que si no sabes de ello te contamos como hacerlo. <br>*Cualquier sección adicional tendrá un costo asociado que debemos cotizar en caso de ser requerida.</p>
      </div>
    </section>
    <WaveComp :colorInicial="'#C16BF9'" :colorFinal="'#C16BF9'"/>
    <section id="comofunciona" class="text-center container">
      <h2 class="purple-text">¿Cómo funciona?</h2>
      <div class="row text-center">
        <StepCard 
          :CardNumber="'1'" 
          :CardTittle="'Envíanos toda la información que quieres incorporar'" 
          :CardText="'Según la estructura anterior. Nosotros nos encargamos de aterrizarlo en una maqueta siguiendo tu imagen de marca de una forma genial!'"
        />
        <StepCard 
          :CardNumber="'2'" 
          :CardTittle="'Llevamos todo lo aprobado a tu maqueta digital'" 
          :CardText="'Conectamos con Google Analytics, agregamos el pixel de facebook. Agregamos formulario (si lo necesitas) o linkeamos a la URL donde quieres enviar a tus prospectos.'"
        />
        <StepCard 
          :CardNumber="'3'" 
          :CardTittle="'¿Todo OK? Entonces dejamos online tu landing page.'" 
          :CardText="'Ya puedes atraer a tus potenciales clientes y captar su interés.'"
        />
      </div>
    </section>
    <WaveComp :direction="'invertir'" :colorInicial="'#EEEDF0'" :colorFinal="'#EEEDF0'"/>
    <section class="container-fluid" id="reviews">
      <div class="container text-center">
        <h2 class="purple-text">
          Esto dicen de nosotros
        </h2>
        <div class="row">
          <div class="col-xl-4 step-cont">
            <div class="card align-items-center">
              <img src="../assets/remax.png" alt="" class="card-img-top logo-cliente">
              <div class="card-body">
                <p class="card-title mini-title">Remax Central</p>
                <p class="card-text medium-p sans">Verónica Irarrázaval</p>
                <p class="card-text mini-little-p">
                  Me encantó trabajar con Vanilla, ya que rápidamente captaron la idea de lo que estábamos buscando, con una excelente disposición a encontrar las soluciones de nuestros requerimientos.
                </p>
                <a href="https://www.elcambioqueesperas.cl" class="btn btn-purple" target="_blank">www.elcambioqueesperas.cl</a>
              </div>
            </div>
          </div>
          <div class="col-xl-4 step-cont">
            <div class="card align-items-center">
              <img src="../assets/futuropat.png" alt="" class="card-img-top logo-cliente">
              <div class="card-body">
                <p class="card-title mini-title">Futuro Patagonia</p>
                <p class="card-text medium-p sans">Mario Ureta</p>
                <p class="card-text mini-little-p">
                  Pendiente
                </p>
                <a href="https://www.futuropatagonia.cl" class="btn btn-purple" target="_blank">www.futuropatagonia.cl</a>
              </div>
            </div>
          </div>
          <div class="col-xl-4 step-cont">
            <div class="card align-items-center">
              <img src="../assets/joaquin.png" alt="" class="card-img-top logo-cliente">
              <div class="card-body">
                <p class="card-title mini-title">Amigos de Joaquín</p>
                <p class="card-text medium-p sans">Javiera</p>
                <p class="card-text mini-little-p">
                  Pendiente
                </p>
                <a href="https://www.amigosdejoaquin.cl" class="btn btn-purple" target="_blank">www.amigosdejoaquin.cl</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <WaveComp :colorInicial="'#EEEDF0'" :colorFinal="'#EEEDF0'"/>
    <section id="nosotros">
      <div class="container text-center">
        <h2 class="purple-text">
          Algo sobre nosotras
        </h2>
        <div class="row container mx-auto">
          <div class="col-12 col-lg-3 us-cont">
            <img src="../assets/icons/cohete.png" alt="cohete">
            <p class="medium-p">Más de 10 años apoyando negocios y marcas.</p>
          </div>
          <div class="col-12 col-lg-3 us-cont">
            <img src="../assets/icons/carita.png" alt="caritas">
            <p class="medium-p">Más de 50 negocios atendidos en los últimos años.</p>
          </div>
          <div class="col-12 col-lg-3 us-cont">
            <img src="../assets/icons/grl_pwr.png" alt="audifonos">
            <p class="medium-p">Somos un equipo de mujeres apasionadas por los desafíos.</p>
          </div>
          <div class="col-12 col-lg-3 us-cont">
            <img src="../assets/icons/estrellas.png" alt="estrellas">
            <p class="medium-p">1000% comprometidas con  que vivas una gran experiencia.</p>
          </div>
        </div>
      </div>
    </section>
    <WaveComp :direction="'invertir'"/>
    <section id="cta" class="container-fluid">
      <div class="container d-flex justify-content-between mx-auto cta-box">
        <h3 class="white-text bold d-lg-inline d-block text-lg-start text-center">¿Tu negocio necesita<br><span class="no-bold">expresar lo genial que es?</span></h3>
        <img src="../assets/white_arrow.svg" alt="flecha curva" class="d-xl-block d-none purple-arrow">
        <FuchsiaButton :buttonText="'¡Trabajemos juntos!'" class="d-block mt-5"/>
      </div>
    </section>
    <WaveComp/>
    <section id="somos">
      <div class="container text-center">
        <h2 class="purple-text">Somos</h2>
        <div class="row">
          <div class="col-xl-4 mb-xl-0 mb-3">
            <img src="../assets/michelle.png" alt="">
          </div>
          <div class="col-xl-8 text-xl-start">
            <p class="mini-title">Michelle De Dompierre</p>
            <p class="bajada">Fundadora de Vanilla Diseño</p>
            <p class="medium-p mt-3">Soy titulada de Diseño Industrial, Diplomada de Marketing Estratégico y me encanta permanecer en constante aprendizaje de nuevas herramientas, tendencias y habilidades. Estoy convencida que el aporte de diseño potencia enormemente a los negocios, no solo de cara al cliente y consumidor, sino que también juega un papel muy relevante en la confianza del equipo sobre la marca.</p>
          </div>
        </div>
        <div class="row">
          <div class="col-xl-4 order-xl-1 order-0 m-xl-0 my-3">
            <img src="../assets/jesu.png" alt="">
          </div>
          <div class="col-xl-8 text-xl-end order-xl-0 order-1">
            <p class="mini-title">María Jesús Petour</p>
            <p class="bajada">Desarrollo y gestión de proyectos</p>
            <p class="medium-p mt-3">Como la persona curiosa y activa que soy, siempre estoy buscando cosas nuevas que aprender, como deportes, manualidades, tecnologías, etc. Estudié Ingeniería Comercial y los últimos años he explorado el mundo digital, donde vinculando mi creatividad con mi capacidad organizacional he aprendido nuevas herramientas y desarrollado grandes proyectos, sobre todo durante la pandemia, donde estudié Desarrollo Front End aprendiendo herramientas como JavaScript, HTML y CSS.</p>
          </div>
        </div>
      </div>
    </section>
    <WaveComp :direction="'invertir'" :colorInicial="'#EEEDF0'" :colorFinal="'#EEEDF0'"/>
    <section class="container-fluid" id="preguntas">
      <div class="container text-center">
        <h2 class="purple-text">
          ¿Tienes dudas?
        </h2>
        <div class="accordion" id="accordionFaqs">
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse1" aria-expanded="true" aria-controls="#collapse1">
                Pregunta 1
              </button>
            </h2>
            <div id="collapse1" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body medium-p text-start">
                Respuesta 1
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse2" aria-expanded="true" aria-controls="#collapse2">
                Pregunta 2
              </button>
            </h2>
            <div id="collapse2" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body medium-p text-start">
                Respuesta 2
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse3" aria-expanded="true" aria-controls="#collapse3">
                Pregunta 3
              </button>
            </h2>
            <div id="collapse3" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body medium-p text-start">
                Respuesta 3
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <WaveComp :colorInicial="'#EEEDF0'" :colorFinal="'#EEEDF0'"/>
    <section id="lanzamiento">
      <div class="text-center container">
        <h2 class="purple-text">Tenemos precio de lanzamiento</h2>
        <p><span class="pink-text big-text">$167.000 +iva </span><span class="tachado">$257.000 + iva</span></p>
        <p class="little-text mb-4">¡Solo 10 cupos a este precio!</p>
        <a 
          href="#tally-open=3NXjAj&tally-layout=modal&tally-width=386&tally-emoji-text=💜&tally-emoji-animation=heart-beat&tally-auto-close=6000" 
          class="fuchsia-text little-text"
        >QUIERO MI DISEÑO DE LANDING PAGE</a>
      </div>
    </section>
    <footer class="container text-center">
      <img src="../assets/logo_footer.png" alt="">
    </footer>
  </div>
</template>

<script>
// @ is an alias to /src
import PreHeader from '@/components/PreHeader.vue'
import FuchsiaButton from '@/components/FuchsiaButton.vue'
import WaveComp from '@/components/WaveComp.vue'
import StepCard from '@/components/StepCard.vue'


export default {
  name: 'HomeView',
  components: {
    PreHeader,
    FuchsiaButton,
    WaveComp,
    StepCard,
  }
}
</script>
