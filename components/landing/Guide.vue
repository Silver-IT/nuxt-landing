<template>
  <p class="mt-8 mx-10 mb-5 text-center text-xl">{{guides[selection]}}</p>
</template>

<script>
export default {
  name: 'LandingGuide',
  props: {
    selection: {
      type: Number,
      default: 0
    }
  },
  data () {
    return {
      guides: [
        'Drei einfache Schritte zu deinem neuen Job',
        'Drei einfache Schritte zur deinem neuen Mitarbeiter',
        'Drei einfache Schritte zur Vermittlung neuer Mitarbeiter'
      ]
    }
  }
}
</script>

<style scoped>
p {
    color: #4A5568;
}
</style>
