<script>
import Trending from './Trending.vue';
</script>

<template>
<div 
    class="
        grid
        grid-cols-1
        rounded-3xl
        bg-gray-800
        w-[350px]
        h-[450px]
    ">

    <span class="
        font-bold
        px-[16px]
        pt-[16px]
        pb-[8px]
    ">
        What's happening
    </span>

    <Trending class="px-[16px] py-[8px] hover:bg-gray-700"/>
    <Trending class="px-[16px] py-[8px] hover:bg-gray-700"/>
    <Trending class="px-[16px] py-[8px] hover:bg-gray-700"/>
    <Trending class="px-[16px] py-[8px] hover:bg-gray-700"/>

    <span class="
    text-[14px]
        text-sky-600
        hover:bg-gray-700
        px-[16px]
        rounded-b-3xl
    ">
        Show more
    </span>
</div>
</template>