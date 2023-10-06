<template>
    <center>
    <button class="button-page" aling="">Mi Vlog</button>
    </center>
</template>

<script lang="ts">
    import { defineComponent, DefineComponent } from 'vue';

    export default defineComponent({
        name: "buttonPage"
    })
</script>

<style lang="scss" scoped>
.button-page {
    background-color: aqua;
    padding: 5px;
    border: solid 1px rgb(255, 0, 0);
    &:hover{
        background-color: blue;
        border: solid px aqua;
        color: #FFFFFF;
    }
}
</style>