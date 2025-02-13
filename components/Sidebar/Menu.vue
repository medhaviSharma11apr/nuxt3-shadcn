<script setup>
const loading = ref(false);
const open = ref(true);
const items = ref([
      {
        title: "Overview",
        path: "/",
        icon: "ri:dashboard-line",

    },
    {
        title: "Transactions",
        path: "/transactions",
        icon: "grommet-icons:transaction",
    },
    {
        title: "Account",
        path: "/account",
        icon: "tdesign:setting",
    },
    {
        title: "Contacts",
        path: "/contacts",
        icon: "mdi:contact-outline",
    },
    {
        title: "Setting",
        path: "/setting",
        icon: "solar:settings-outline",
    },
])
</script>

<template>
    <div> 
        <header class="flex items-center gap-2 p-4 hover:scale-[105%] transition cursor-pointer  ">
            <Logo></Logo>
            <p class="font-bold">Deepak Mishra</p>
            
        </header>
        <div class="px-4 grow">
                <div class="grid gap-4">
                    <div v-for="(item , index) in items " :key="index" class="flex item-center gap-2 px-2 py-1 transition rounded cursor-pointer hover:bg-neutral-100">
                        <Icon :name="item.icon" class="mt-1" size="20" co></Icon>
                        <span>
                            {{
                                item.title
                            }}
                        </span>
                       
                    </div>
                </div>
            </div>
    </div>
</template>