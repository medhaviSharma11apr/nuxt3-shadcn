<script setup>
const loading= ref(false)
</script>

<template>
 <div class="grid item-start ">
    <div>
        <Sidebar></Sidebar>
    </div>

    <div>
         <slot></slot>
    </div>

 </div>
</template>