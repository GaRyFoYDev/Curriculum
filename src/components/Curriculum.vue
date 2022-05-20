<template>
<div class="container">
    <Left  class="left_container"/>
    <Right class="right_container" />
</div>

</template>

<script setup lang="ts">

import Left from "./left.vue";
import Right from "./right.vue";

</script>




<style lang="scss" scoped>

.container{
    background-color: var(--white);
    width: 65%;
    min-height: 100vh;
    margin: 50px auto;
    box-shadow: 0px 30px 40px rgba(0,0,0,0.3);
    display: flex;

@media screen and (max-width: 768px) {
    width: 90%;
    flex-direction: column;
}
 
   
}


</style>