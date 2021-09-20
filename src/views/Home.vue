<template>
  <div class="home">
    <h1 style='font-size: 3rem'>Resolução Maxima: {{w}} X {{h}}</h1>
    <h1 style='font-size: 3rem'>Resolução do Sistema: {{w2}} X {{h2}}</h1>
    <h1 style='font-size: 3rem'>Resolução da Janela: {{w3}} X {{h3}}</h1>
  </div>
</template>

<script>

export default {
  name: 'Home',

  data () {
    return {
      w: 0,
      h: 0,
      h2: 0,
      w2: 0,
      h3: 0,
      w3: 0
    }
  },

  mounted () {
    this.h = window.screen.availHeight
    this.w = window.screen.availWidth
    this.h2 = window.screen.height
    this.w2 = window.screen.width
    this.h3 = window.innerHeight
    this.w3 = window.innerWidth
  }
}
</script>
