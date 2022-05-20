<template>
  <section class="agreement-wrapper">
    <Header />
    <p class="text-center text-5xl py-5 bg-transparent">Deine Job website</p>
    <div
      class="agreement-image flex justify-center h-96 bg-no-repeat bg-center"
    ></div>
    <div class="register-wrapper bg-white rounded-t-xl p-6 mb-12">
      <div
        class="
          btn-register
          p-3
          text-center
          rounded-xl
          text-white
          cursor-pointer
        "
      >
        Kostenlos Registrieren
      </div>
    </div>
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

.agreement-image {
  background-image: url("/undraw_agreement_aajr.svg");
}

.register-wrapper {
  box-shadow: 0px -1px 3px #00000033;
}

.btn-register {
  background: transparent linear-gradient(95deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
}
</style>