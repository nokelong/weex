<template>
   <div class="wrapper">
   	  <label class="txt">what you want say for me</label>
   	  <input type='text' class='input' ref='input' v-on:input='oninput' />
   </div>
</template>
<style>
    .input {
        font-size: 50px;
        width: 650px;
        margin-top: 50px;
        margin-left: 50px;
        padding-top: 20px;
        padding-bottom: 20px;
        padding-left: 20px;
        padding-right: 20px;
        color: #666666;
        border-width: 2px;
        border-style: solid;
        border-color: #41B883;
    }
    .txt{
    	color: green;
        font-size: 50px;
    }

</style>
<script>
  const modal = weex.requireModule('modal')
  export default {  	
  	methods:{
       oninput (event){
          console.log('oninput:', event.value);
          modal.toast({
          	message:'oninput:${event.value}',
          	duration: 0.8
          })
       }
  	}
  }
</script>