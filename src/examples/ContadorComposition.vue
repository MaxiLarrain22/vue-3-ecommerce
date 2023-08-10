<script setup lang="ts">
    import { onMounted, ref } from 'vue'

    const count = ref(0);

    function aumentar(){

        count.value +=1
        
    }

    onMounted(function() {
        console.log( "El valor inicial del contador es:" + count.value)
    });
    
    // onMounted(() => { Es la misma sintaxis
    //     console.log( "El valor inicial del contador es:" + count.value)
    // });
</script>


<template>
    <div>
        <h2>Hola soy una version con composition Api</h2>
        <h1>Contador: {{ count }}</h1>
        <button @click="aumentar">
            Incrementar contador
        </button>
    </div>
</template>