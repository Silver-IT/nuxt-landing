<template>
  <div class="flex pl-2 py-5 pr-8 items-end">
    <p class="flex-auto text-9xl -mb-3">1.</p>
    <div class="flex flex-col">
      <img src="/undraw_Profile_data_re_v81r.svg" >
      <p class="pl-5 pt-5">{{labels[selection]}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LandingMakeProfile',
  props: {
    selection: {
      type: Number,
      default: 0
    }
  },
  data () {
    return {
      labels: [
        'Erstellen dein Lebenslauf',
        'Erstellen dein Unternehmensprofil',
        'Erstellen dein Unternehmensprofil'
      ]
    }
  }
}
</script>

<style scoped>
p {
  color: #718096;
}
</style>
