<script setup>
const loading= ref(false)
const open= ref(false)
const toggleopen = ()=>{
    open.value= !open.value;
}
</script>

<template>
  
 <div class="relative"> 
      <!-- mobile -->
    <div class="z-50 flex lg:hidden item-center justify-between w-full h-full p-4">
      <Logo></Logo>
      <Icon class="z-50 cursor-pointer left-2 top-2  " size="30" name="iconamoon:menu-burger-horizontal" @click="toggleopen()"></Icon>

      <div v-if="open" class="fixed top-0 left-0 z-50 w-full h-full h-screen bg-white">
          
          <Icon class="absolute z-50 cursor-pointer right-4 top-4 " size="30" name="line-md:close" @click="toggleopen()"></Icon>
          <SidebarMenu ></SidebarMenu>
      </div>
     
    
    </div>
      <!-- desktop -->
    <div class="hidden lg:flex w-[250px] h-screen flex flex-col justify-between border-r">
        
        <SidebarMenu></SidebarMenu>
        <div>
            User Item
        </div>
    </div>
</div>
</template>