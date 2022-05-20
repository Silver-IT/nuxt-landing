<template>
  <div class="payment-wrapper pt-4 pl-5 pr-5 pb-28 flex flex-col items-center">
    <div class="flex items-end pl-7">
      <p class="text-9xl mr-5">3.</p>
      <p class="flex-auto">{{labels[selection]}}</p>
    </div>
    <img :src="images[selection]" class="mt-7" />
  </div>
</template>

<script>
export default {
  name: 'LandingPayment',
  props: {
    selection: {
      type: Number,
      default: 0
    }
  },
  data () {
    return {
      labels: [
        'Mit nur einem Klick bewerben',
        'Wahle deinen neuen Mitarbeiter aus',
        'Vermittlung nach Provision oder Stundenlohn'
      ],
      images: [
        '/undraw_personal_file_222m.svg',
        '/undraw_swipe_profiles1_i6mr.svg',
        '/undraw_business_deal_cpi9.svg'
      ]
    }
  }
}
</script>

<style scoped>
.payment-wrapper {
  color: #718096;
}
</style>
