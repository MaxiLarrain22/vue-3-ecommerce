
<script lang="ts">
// Options API
// Con un contador definimos el estado de nuestro componente
export default {

    data(){

        return {

            count:0

        }
    },

    methods:{

        increase(){

            this.count += 1; // Es equivalente a this.count = this.count +1;

        }
    },
    // mounted sirve para mostrar un mensaje
    mounted(){

       console.log ("El valor inicial es: " + this.count)

    }
}
</script>


<template>

  <h1>Contador: {{ count }} </h1>
  <button @click="increase">
    Aumentar contador
  </button>
  
</template>

