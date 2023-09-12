<template>
<button @click="click">dianji</button>
</template>

<script>
 export default {
   name:'ThreeSasdf',
 methods:{
  click(){
      this.$emit('agree','我是three的消息！')
    }
   }
 }
</script>
