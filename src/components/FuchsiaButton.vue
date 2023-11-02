<template>
  <button 
    type="button"
    class="btn btn-fuchsia rounded-pill"
    data-tally-open="3NXjAj" data-tally-layout="modal" data-tally-emoji-text="💜" data-tally-emoji-animation="heart-beat"
  >
    <router-link :to="to">{{buttonText}}</router-link>
  </button>
</template>

<script>

export default {
  name: 'FuchsiaButton',
  props: {
    to: {
      type: String,
      default: '/'
    },
    buttonText: {
      type: String,
      default: 'Button'
    }
  }
}
</script>
