<template>
  <section class="hero is-dark is-fullheight">
    <div class="hero-head">
      <Navbar />
    </div>
    <div class="hero-body">
      <div class="container">
        <p class="title">
          // Justin Cheung
        </p>
        <p class="subtitle">
          Software Developer / Goose Watcher
        </p>
        <!-- TODO
        <b-button icon-left="information" tag="router-link" to="/about" type="is-dark" rounded>
          About Me
        </b-button>
        -->
        <b-button icon-left="file-document" tag="a" href="docs/resume.pdf" type="is-dark" rounded>
          Resume
        </b-button>
      </div>
    </div>
    <div class="hero-footer">
      <Footer />
    </div>
  </section>
</template>

<script>
export default {
  head() {
    return {
      script: [
        {
          src: 'https://identity.netlify.com/v1/netlify-identity-widget.js'
        }
      ],
      title: 'Justin Cheung'
    };
  },
}
</script>

<style scoped>
.hero {
  background: linear-gradient( rgb(0 0 0 / 25%), rgb(0 0 0 / 25%) ), url('/img/uw_campus_canada_goose.JPG');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.footer {
  background: transparent;
}
</style>
