<script>
import PotentialFollowers from './PotentialFollowers.vue';
</script>

<template>
<div 
    class="
        grid
        grid-cols-1
        rounded-3xl
        bg-gray-800
        w-[350px]
        h-[300px]
    ">

    <span class="font-bold px-[16px] pt-[16px] pb-[8px]">
        You might like
    </span>

    <div class="grid grid-cols-1">
        <PotentialFollowers 
            class="px-[16px] py-[8px] hover:bg-gray-700"
            imageUrl="https://picsum.photos/200/200?a"
            profilename="John Doe"
            username="johndoe"/>
        <PotentialFollowers 
            class="px-[16px] py-[8px] hover:bg-gray-700"
            imageUrl="https://picsum.photos/200/200?b"
            profilename="Jane Doe"
            username="janedoe"/>
        <PotentialFollowers 
            class="px-[16px] py-[8px] hover:bg-gray-700"
            imageUrl="https://picsum.photos/200/200?c"
            profilename="Play Doe"
            username="playdoe"/>
    </div>

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