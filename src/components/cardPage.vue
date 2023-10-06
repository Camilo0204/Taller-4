<template>
    <center>
    <div class="card-page">

        <h3>{{ title }}</h3>
        <p>{{ summary }}</p>
        <img :src="require('@/assets/img/PrimeraGuerraM.png')" alt="100px" >
        <buttonPage />
    </div>
    </center>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import buttonPage from './buttonPage.vue';


export default defineComponent({
    name: "cardPage",
    components: {
        buttonPage
    },
    props: {
        title: {
            type: String,
            default: ""
        },
        summary: {
            type: String,
            default: ""
        },
        imagenURL: {
            type: String, // Asegúrate de que la propiedad imagenURL sea de tipo String
            default: "@/assets/img/PrimeraGuerraM.png" // Cambia esto por una imagen predeterminada si es necesario
        }
    }
})
</script>

<style lang="scss" scoped>
.card-page {
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: solid 1px #ccc;
}
</style>