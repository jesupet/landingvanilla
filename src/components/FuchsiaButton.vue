<template>
  <button 
    type="button"
    class="btn btn-fuchsia rounded-pill"
    data-tally-open="3NXjAj" data-tally-layout="modal" data-tally-width="700" data-tally-emoji-text="👋" data-tally-emoji-animation="wave" data-tally-auto-close="2000"
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
