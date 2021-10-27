<template>
   <span> Hello {{ message }} </span><br/> 
   <span> {{ OnlyFirstWord }} </span><br/> 
   <span v-if="estVisible"> Mon Texte </span>
</template>
<script>
  export default {
     data() {
       return {
          message: "Zoulette World",
          compteur: 13,
          pourcentage: 60,
          estVisible: true,
          tableauVide: []
       }
    },
    computed: {
      OnlyFirstWord() {
        return this.message.split(' ')[0].toUpperCase();
      }
    }
  }
</script>