<template>
  <div>
    <section class="hero is-dark is-halfheight">
      <div class="hero-head">
        <Navbar />
      </div>
      <div class="hero-body">
        <div class="container">
          <p class="title">
            {{ post.title }}
          </p>
          <p class="subtitle">
            {{ post.subtitle }}
          </p>
        </div>
      </div>
    </section>
    <section class="section content-section">
      <div class="container">
        <div class="content">
          <nuxt-content :document="post" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  async asyncData ({ $content }) {
    const post = await $content('about').fetch()
    return {
      post
    }
  },
  head () {
    return {
      title: 'About Me - Justin Cheung'
    }
  }
}
</script>

<style scoped>
.hero {
  background: linear-gradient( rgb(0 0 0 / 25%), rgb(0 0 0 / 25%) ), url('/img/glowing-pokeball.JPG');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
</style>
