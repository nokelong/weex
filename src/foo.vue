<template>
  <div class="wrapper" @click="update">
    <head></head>
    <input></input>
  </div>  
</template>

<style>
  .wrapper { align-items: center; margin-top: 120px; }
  .title { font-size: 48px; }
  .logo { width: 360px; height: 82px; }
</style>

<script>
  import head from './head.vue'
  import input from './input.vue'

  export default {
    data: {
      logoUrl: 'https://alibaba.github.io/weex/img/weex_logo_blue@3x.png',
      target: 'World'
    },
    components:{head,input},
    methods: {
      update: function (e) {
        this.target = 'Weex'
        console.log('target:', this.target)
      }
    }
  }
</script>
