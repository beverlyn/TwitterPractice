<script setup lang="ts">
import PhotoGrid from './components/PhotoGrid.vue';
import YouMightLike from "./components/YouMightLike.vue";
import WhatsHappening from "./components/WhatsHappening.vue"
</script>

<template>
<div
    class="
        text-[20px]
        w-[350px]
    ">
    <div
        class="
        fixed
        top-0
        bg-black
        h-[56px]
    ">
        <div
            class="
                text-[16px]
                bg-gray-700
                rounded-full
                w-[350px]
                p-[12px]
                m-[4px]
        ">
            Search
        </div>
    </div>

    <div
        class="
            grid
            grid-cols-1
            gap-[16px]
    ">
        <PhotoGrid class="mt-[68px]"/>
        <YouMightLike />
        <WhatsHappening />
    </div>
</div>
</template>