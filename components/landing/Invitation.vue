<template>
  <div
    class="
      invitation-wrapper
      relative
      inline-block
      w-full
      align-middle
      overflow-hidden
      pt-16
      pl-7
      pr-5
      pb-20
    "
  >
    <svg
      class="wavy-top"
      viewBox="0 0 500 500"
      preserveAspectRatio="xMinYMin meet"
    >
      <path
        d="M0,100 C150,200 350,0 500,100 L500,0 L0,0 Z"
        style="stroke: none; fill: white"
      ></path>
    </svg>
    <div class="flex items-end">
      <p class="text-9xl mr-5">2.</p>
      <p class="flex-auto mb-3">{{labels[selection]}}</p>
    </div>
    <div class="flex justify-center">
      <img :src="images[selection]" class="float-right mr-5" />
    </div>
    <svg
      class="wavy-bottom"
      viewBox="0 0 500 250"
      preserveAspectRatio="xMinYMin meet"
    >
      <path
        d="M0,150 C150,250 350,50 500,150 L500,250 L0,250 Z"
        style="stroke: none; fill: white"
      ></path>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'LandingInvitation',
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
        'Erstellen ein Jobinserat',
        'Erhalte Vermittlungsangebot von Arbeitgeber'
      ],
      images: [
        '/undraw_task_31wc.svg',
        '/undraw_about_me_wa29.svg',
        '/undraw_job_offers_kw5d.svg'
      ]
    }
  }
}
</script>

<style scoped>
svg.wavy-top {
  display: inline-block;
  position: absolute;
  top: -50px;
  left: 0;
}

svg.wavy-bottom {
  display: inline-block;
  position: absolute;
  bottom: -50px;
  left: 0;
}

.invitation-wrapper {
  background: transparent linear-gradient(134deg, #e6fffa 0%, #ebf4ff 100%) 0%
    0% no-repeat padding-box;
  color: #718096;
}
</style>
