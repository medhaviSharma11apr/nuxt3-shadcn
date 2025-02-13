<script setup>
const loading= ref(false)
</script>

<template>
 <div class="flex item-start ">
    <div>
        <Sidebar></Sidebar>
    </div>

    <div>
         <slot></slot>
    </div>

 </div>
</template>