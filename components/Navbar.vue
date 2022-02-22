<template>
  <b-navbar spaced>
    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        // Justin Cheung
      </b-navbar-item>
      <b-navbar-item href="mailto:me@j43cheun.dev">
        <b-icon icon="email" />
      </b-navbar-item>
      <b-navbar-item href="https://github.com/j43cheun">
        <b-icon icon="github" />
      </b-navbar-item>
      <b-navbar-item href="https://www.linkedin.com/in/j43cheun">
        <b-icon icon="linkedin" />
      </b-navbar-item>
      <b-navbar-item href="docs/resume.pdf">
        <b-icon icon="file-document" />
      </b-navbar-item>
    </template>
    <!-- TODO
    <template #end>
      <b-navbar-item tag="router-link" :to="{ path: '/about' }">
        About
      </b-navbar-item>
    </template>
    -->
  </b-navbar>
</template>

<style scoped>
.is-circular {
  border-radius: 50%
}
</style>
