<script setup lang="ts">
defineProps({
    imageUrl: String,
    profilename: String,
    username: String,
})
</script>

<template>
<div class="potentialFollows">
    <img 
        :src="imageUrl" 
        class="w-[50px] h-[50px] rounded-md"
    />
    <span>
        <p class="
            font-bold
            text-[16px]
            hover:underline
        ">
            {{ profilename }}
        </p>
        <p class="
            text-[14px]
            text-neutral-500
        ">
            @{{ username }}
        </p>
    </span>

    <button class="
            bg-white
            rounded-full
            text-black
            text-[14px]
            hover:bg-gray-400
            font-bold
            w-[80px]
            h-[30px]
    ">
        Follow
    </button>
</div>
</template>

<style>
.potentialFollows {
    display: grid;
    grid-template-columns: 50px 150px 80px;
    gap: 16px;
    align-items: center;
}
</style>
