<script setup>
const loading= ref(false)
definePageMeta(
    {
        layout:"custom"
    }
)
</script>

<template>
 <div>  
    custom component layout 
    <slot/>
</div>
</template>