<template>
  <WhatsAppBtn class="whatsapp fixed-button" :v-if="showButton"/>
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
        <p class="white-text">Precio lanzamiento: <span class="pink-text big-text d-none">$167.000 +iva </span><span>$287.000 + iva</span></p>
        <FuchsiaButton :buttonText="'Quiero mi landing page'" class="my-4"/>
        <p class="little-text white-text d-none">¡Solo 10 cupos a este precio!</p>
        <p class="little-text white-text pt-5">*Incluye un año de <a href="#preguntas" class="underline">modificaciones de contenido</a> sin costo.</p>
        <p class="little-text white-text">*El precio no incluye dominio y hosting, debes tenerlo tu. Pero no te preocupes que si no sabes de ello <a href="#preguntas" class="underline">te contamos como hacerlo</a>.</p>
        <p class="little-text white-text" >*Cualquier sección adicional tendrá un costo asociado que debemos cotizar en caso de ser requerida.</p>
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
                  Después de tomar la decisión de trabajar con Vanilla, creo no haberme equivocado ya que cumplieron con todas mis expectativas. Respecto al diseño, muy ingenioso y cumplieron con los tiempos comprometidos en un principio.
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
                  La conocí, le conté lo que queríamos y necesitábamos y en tan solo unos días me presentó una página web hermosa. Cálida, delicada y llena de detalles que la hicieron completamente nuestra. Gracias Vanilla por el compromiso y el profesionalismo en todo momento. Gracias por ser parte de amigos de Joaquín ❤️
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
                ¿Para qué sirve tener un landing page?
              </button>
            </h2>
            <div id="collapse1" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  Un Landing page es una “página web de aterrizaje” y está diseñada para una acción específica. 
                  Es decir enfocada en un sólo objetivo, como puede ser: <span class="purple-text">capturar leads, promocionar un servicio, un evento u otro similar.</span><br><br>
                  ¡Es simple y directo!<br><br>
                  Recuerda, un <span class="purple-text">landng page</span> es como una carta de amor apasionada, mientras que un <span class="purple-text">sitio web</span> es como un libro completo. ¡Ambos son esenciales, pero para diferentes propósitos!
                </p> 
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse2" aria-expanded="true" aria-controls="#collapse2">
                ¿Quién realiza el contenido para mi landing page?
              </button>
            </h2>
            <div id="collapse2" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  Nadie mejor que tú conoce el negocio, y es por ello que es importante tener claro lo que quieres transmitir con esta página, y para eso <span class="purple-text">debes entregarnos el contenido (textos, componentes de marca e imágenes)</span>  que quieres disponer en él, y al que nosotros le daremos toda la genialidad y diseño para mostrar de una forma clara y atractiva eso que quieres decir.<br><br>
                  En un comienzo te mandaremos una “estructura tipo”, que puede servirte de apoyo para crear ese contenido, y finalmente al tenerlo en nuestras manos, también te haremos sugerencias en caso de ver que puedes sacar un mayor provecho de él.<br><br>
                  De todas formas, <span class="purple-text">si necesitas que desarrollemos ese contenido porque no tienes el tiempo suficiente, ¡no es problema!</span> cuéntanos y realizaremos una cotización para apoyarte con ello.
                </p>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse3" aria-expanded="true" aria-controls="#collapse3">
                ¿Cuántas modificaciones/iteraciones tendremos para el proyecto?
              </button>
            </h2>
            <div id="collapse3" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  La idea de este servicio es ir rápido pero seguro y eficaz.<br><br>
                  En ese sentido esperamos generar <span class="purple-text">la menor cantidad de iteraciones posibles</span>. Para ello es importante que tengas el tiempo de revisar con detalle las entregas que realizaremos, para que cumplamos las expectativas que tienes y todo funcione genial.<br><br>
                  Un ejemplo detallado del proceso sería:
                  <ul>
                    <li class="medium-p">
                      1. Reunión inicial de bienvenida y levantamiento de información.
                    </li>
                    <li class="medium-p">
                      2. Recepción del material que te solicitamos.
                    </li>
                    <li class="medium-p">
                      3. Entrega de propuesta de diseño para tu landing page, junto a recepción de feedback y/o dudas.
                    </li>
                    <li class="medium-p">
                      4. Entrega final de diseño.
                    </li>
                    <li class="medium-p">
                      5. Montaje de tu landing page en HTML, CSS y JS.
                    </li>
                    <li class="medium-p">
                      6. Integración de Whatsapp, Analytics, formulario de contacto y/o CRM.
                    </li>
                    <li class="medium-p">
                      7. Puesta on-line de tu landingpage.
                    </li>
                  </ul>
                </p>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse7" aria-expanded="true" aria-controls="#collapse7">
                ¿Puedo modificar yo misma el contenido de mi landing page?
              </button>
            </h2>
            <div id="collapse7" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  <span class="purple-text">Tu landing lo construimos desde cero</span>, eso quiere decir que el diseño es único y puedes expandirlo más adelante a un sitio web propiamente tal, sin problema. 
                  <br>
                  Si necesitas modificar algo no te preocupes, lo haremos nosotros por ti, <span class="purple-text">incluimos un año gratis de modificaciones!</span>
                  <br>
                  Con esto incluimos lo siguiente:
                  <br><br>
                  <ul>
                    <li class="medium-p">
                      Editar o agregar recomendaciones/testimonios de tus clientes
                    </li>
                    <li class="medium-p">
                      Agregar o eliminar fotos 
                    </li>
                    <li class="medium-p">
                      Editar datos de contacto
                    </li>
                  </ul>
                </p>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse4" aria-expanded="true" aria-controls="#collapse4">
                No tengo hosting y/o dominio. ¿Qué debo hacer?
              </button>
            </h2>
            <div id="collapse4" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  Te comentamos los pasos a seguir para obtener estos elementos que son indispensables para el proyecto.<br><br>
                  Te podemos recomendar:<br><br>
                </p>
                  <ul>
                    <li class="medium-p">
                      Contratación dominio .cl: <a href="https://www.nic.cl" class="purple-text" target="_blank">https://www.nic.cl</a> 
                    </li>
                    <li class="medium-p">
                      Contratación dominio .com: <a href="https://www.godaddy.com/es" class="purple-text" target="_blank">https://www.godaddy.com/es</a> 
                    </li>
                    <li class="medium-p">
                      Contratación hosting + dominio .cl: <a href="https://www.solucionhost.cl" class="purple-text" target="_blank">hhttps://www.solucionhost.cl</a> 
                    </li>
                  </ul>
                 <p class="medium-p">Si en definitiva este tema para ti es chino mandarín y quieres que nosotras lo veamos, no te preocupes que podemos hacerlo. Estos son los costos asociados: <br><br>
                  Gestión Vanilla: <span class="purple-text">1 UF + los costos de lo que requieras contratar:</span> <br><br>
                 </p>
                  <ul>
                    <li class="medium-p">
                      Contratación dominio .cl: $9.990 + IVA Anual 
                    </li>
                    <li class="medium-p">
                      Contratación dominio .com: dependerá del nombre del sitio 
                    </li>
                    <li class="medium-p">
                      Contratación hosting básico: desde $11.990
                    </li>
                  </ul>
                  <br>
                  *Precios sujetos a confirmación al momento de la contratación del servicio
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse5" aria-expanded="true" aria-controls="#collapse5">
                ¿Cuánto demora el proyecto en estar online?
              </button>
            </h2>
            <div id="collapse5" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  El tiempo de desarrollo lo tenemos programado para <span class="purple-text">3 a 4 semanas</span>. Mientras más claro tengas el contenido y lo que quieres lograr, más ágil podemos desarrollar el proceso.
                </p>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <h2 class="accordion-header">
              <button class="accordion-button medium-p" type="button" data-bs-toggle="collapse" data-bs-target="#collapse6" aria-expanded="true" aria-controls="#collapse6">
                ¿Qué medios de pago hay?
              </button>
            </h2>
            <div id="collapse6" class="accordion-collapse collapse" data-bs-parent="#accordionFaqs">
              <div class="accordion-body text-start">
                <p class="medium-p">
                  Puedes pagar con una <span class="purple-text">transferencia</span> a nuestra cuenta corriente. Pagas un 50% al comienzo y el 50% al finalizar contra-entrega.
                </p>
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
        <p><span class="pink-text big-text d-none">$167.000 +iva </span><span>$287.000 + iva</span></p>
        <p class="little-text mb-4 d-none">¡Solo 10 cupos a este precio!</p>
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
import WhatsAppBtn from '@/components/WhatsAppBtn.vue'


export default {
  name: 'HomeView',
  components: {
    PreHeader,
    FuchsiaButton,
    WaveComp,
    StepCard,
    WhatsAppBtn,
  }
}
</script>
