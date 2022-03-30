<template>
  <h1 data-animation="fade-in">Hello Motion UI</h1>
</template>

<script>
import $ from 'jquery'

const component = {
  mounted() {
    const $element = $('h1')

    $element.click(() => {
      Foundation.Motion.animateIn($element, 'fade-in')
    })
  },
}

export default component
</script>
