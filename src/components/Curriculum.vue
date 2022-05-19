<template>
<div class="container">
    <Left  class="container_left"/>
    <Right class="container_right" />
</div>

</template>

<script setup lang="ts">

import Left from "./left.vue";
import Right from "./right.vue";

</script>




<style lang="scss" scoped>

.container{
    background-color: var(--white);
    width: 50%;
    height: 100vh;
    margin: 50px auto;
    box-shadow: 0px 30px 40px rgba(0,0,0,0.3);
    display: flex;

    &_left{
        width: 70%;
        height: 100%;
        background-color: var(--grey-2);
    }
}


</style>