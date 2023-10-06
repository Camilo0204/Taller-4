<template>
  <h1>Mi Vlog</h1>
  <ContainerPage/>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import ContainerPage from './components/containerPage.vue';
import cardPage from './components/cardPage.vue';


export default defineComponent({
  components: {
    
    ContainerPage
}
})
</script>

<style lang="scss">

</style>