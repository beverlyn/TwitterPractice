<template>
<div 
    class="
    whatsHappening
">
    <div class="text-[12px] self-center">
        <p class="text-neutral-500">
            Trending in Japan
        </p>
        <p class="text-[16px] font-bold">
            Hashtag
        </p>
        <p class="text-neutral-500">
            10K posts
        </p>
    </div>
    <div>
        <button class="
            rounded-full 
            hover:bg-sky-600/40
            hover:text-sky-300
            p-[8px]
        ">
            <IconMingcuteMore1Line/>
        </button>
    </div>

</div>
</template>

<style>
.whatsHappening {
    display: grid;
    grid-template-columns: 90% 10%;
}
</style>