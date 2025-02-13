<script setup>
const loading= ref(false)
</script>

<template>
 <div class="grid item-start lg:flex ">
    <div>
        <Sidebar></Sidebar>
    </div>

    <div class="p-4">
         <slot></slot>
    </div>

 </div>
</template>