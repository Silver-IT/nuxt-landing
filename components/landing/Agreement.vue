<template>
  <section class="agreement-wrapper pt-16 pb-20">
    <p class="text-center text-5xl py-5 bg-transparent">Deine Job website</p>
    <div
      class="agreement-image flex justify-center h-96 bg-no-repeat bg-center"
    ></div>
    <svg
      class="wavy-bottom"
      viewBox="0 0 500 250"
      preserveAspectRatio="xMinYMin meet"
    >
      <path
        d="M0,200 C150,220 420,80 500,100 L500,250 L0,250 Z"
        style="stroke: none; fill: white"
      ></path>
    </svg>
  </section>
</template>

<script>
export default {
  name: 'LandingAgreement'
}
</script>

<style scoped>
section.agreement-wrapper{
  background: transparent linear-gradient(141deg, #EBF4FF 0%, #E6FFFA 100%) 0% 0% no-repeat padding-box;
}
section.agreement-wrapper p {
  color: #2D3748;
}

svg.wavy-bottom {
  display: inline-block;
  position: absolute;
  bottom: 0;
  left: 0;
}

.agreement-image {
  background-image: url("/undraw_agreement_aajr.svg");
  background-size: cover;
}
</style>