<template>
   <span> Hello {{ message }} </span>
   <span v-if="estVisible"> Mon Texte </span>

</template>
<script>
  export default {
     data() {
       return {
          message: "World",
          compteur: 13,
          pourcentage: 60,
          estVisible: true,
          tableauVide: []
       }
    }
  }
</script>