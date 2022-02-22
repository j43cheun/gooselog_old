<template>
  <div class="site-container">
    <div class="site-content">
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.site-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.site-content {
  flex: 1;
}
</style>

<style lang='scss' scoped>
// Import Bulma and Buefy styles
@import "~bulma/sass/utilities/_all";
@import "~bulma";
@import "~buefy/src/scss/buefy";
</style>
