<template>
  <div>
    <Header />
    <LandingAgreement />
    <section class="mt-5">
      <VueSlickCarousel
        :centerMode="true"
        :centerPadding="'100px'"
        :focusOnSelect="true"
        :slidesToShow="1"
        :speed="500"
        :infinite="false"
        :arrows="false"
      >
        <div
          :class="
            'rounded-l-xl btn-type' + (isEmployeeSelected ? ' btn-focused' : '')
          "
          @click="onClickEmployee"
        >
          Arbeitnehmer
        </div>
        <div
          :class="'btn-type' + (isEmployerSelected ? ' btn-focused' : '')"
          @click="onClickEmployer"
        >
          Arbeitgeber
        </div>
        <div
          :class="
            'rounded-r-xl btn-type' +
            (isContractorSelected ? ' btn-focused' : '')
          "
          @click="onClickContractor"
        >
          Temporarburo
        </div>
      </VueSlickCarousel>
    </section>
    <LandingGuide :selection="selection" />
    <LandingMakeProfile :selection="selection" />
    <LandingInvitation :selection="selection" />
    <LandingPayment :selection="selection" />
    <Footer />
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";

export default {
  name: "IndexPage",
  components: {
    VueSlickCarousel,
  },
  data() {
    return {
      selection: 0,
    };
  },
  computed: {
    isEmployeeSelected() {
      return this.selection === 0;
    },
    isEmployerSelected() {
      return this.selection === 1;
    },
    isContractorSelected() {
      return this.selection === 2;
    },
  },
  methods: {
    onClickEmployee() {
      this.selection = 0;
    },
    onClickEmployer() {
      this.selection = 1;
    },
    onClickContractor() {
      this.selection = 2;
    },
  },
};
</script>

<style scoped>
.btn-type.btn-focused {
  background: #81e6d9 0% 0% no-repeat padding-box;
  color: white;
}
.btn-type {
  color: rgb(45 212 191);
  text-align: center;
  border: 1px solid #cbd5e0;
  padding: 12px;
  cursor: pointer;
}
</style>