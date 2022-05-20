<template>
  <div class="tomisha-header z-10 fixed top-0 left-0 right-0 rounded-b-xl h-16 bg-white">
    <div class="tomisha-header-bar h-1.5"></div>
    <div class="tomisha-header-content flex justify-end p-5">
        <span class="cursor-pointer hover:underline">Login</span>
    </div>
  </div>
</template>

<style scoped>
.tomisha-header {
  box-shadow: 0px 3px 6px #00000029;
}
.tomisha-header-bar {
    background: transparent linear-gradient(91deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
}
.tomisha-header-content {
    color: #319795;
}
</style>
