<template>
  <div class="row text-center">
    <div class="col-xl-3 col-12 step-cont" v-for="(review, index) in reviews" :key="index">
      <div class="card align-items-center">
        <img :src="getImagePath(review.logo)" class="card-img-top icono-pasos" alt="...">
        <div class="card-body">
          <p class="titulo-gris">{{review.marca}}</p>
          <p class="card-text medium-p">{{review.comentario}}</p>
          <PurpleButton :buttonText="(review.boton)"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { mapState } from 'pinia'
import { useCounterStore } from '../store/index'
import PurpleButton from './PurpleButton.vue'

export default {
  name: 'ReviewCard',
  components: {
    PurpleButton,
  },
  computed: {
    ...mapState(useCounterStore, ['reviews'])
  },
  methods: {
    getImagePath(logo) {
      // Utiliza require para cargar la imagen
      return require(`@/assets/${logo}`);
    },
  }
}
</script>