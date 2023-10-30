<template>
  <div class="col-xl-4 col-12 step-cont">
    <div class="card align-items-center">
      <div class="number">
        <h3 class="white-text">{{CardNumber}}</h3>
      </div>
      <div class="card-body">
        <p class="card-title mini-title purple-text">{{CardTittle}}</p>
        <p class="card-text medium-p">{{CardText}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StepCard',
  props: {
    CardNumber: {
      type: String,
      default: '1'
    },
    CardTittle: {
      type: String,
      default: 'Nombre Card'
    },
    CardText: {
      type: String,
      default: 'Texto Card'
    }
  }
}
</script>