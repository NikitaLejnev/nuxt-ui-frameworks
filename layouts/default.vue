<template>
  <div>
    <ul class="menu align-center">
      <li><nuxt-link to="/">Home</nuxt-link></li>
      <li><nuxt-link to="/form">Form</nuxt-link></li>
      <li><nuxt-link to="/motion-ui">Motion UI</nuxt-link></li>
    </ul>
    <Nuxt />
  </div>
</template>

<script>
const component = {
  mounted() {
    this.$getCurrentScreenSize()
  },
}

export default component
</script>
