<template>
    <div class="container-page">
        <card-page v-for="post in posts" :key="post.title"
        
            :title="post.title"
            :summary="post.summary"
            :text="post.text"
            :imagenURL="post.imagenURL"
            
        />
    </div>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import cardPage from './cardPage.vue';
import datos from "@/assets/posts.json";


export default defineComponent({
    name: "containerPage",
    components: {
        cardPage
    },
    computed: {
        posts : ()=>{
            return datos.map((post:any)=>{
                return post
            })
        }
    }
})
</script>

<style lang="scss" scoped>
    .container-page {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }
</style>