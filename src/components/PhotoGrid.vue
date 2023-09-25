<template>
<div 
    class="
        photoGrid
        rounded-xl
        border-[0.5px]
        border-gray-800
        w-[350px]
        h-[200px]
    ">
    <img class= "rounded-tl-xl" src="https://picsum.photos/300/300?a"/>
    <img src="https://picsum.photos/300/300?b"/>
    <img class= "rounded-tr-xl" src="https://picsum.photos/300/300?c"/>
    <img class= "rounded-bl-xl" src="https://picsum.photos/300/300?d"/>
    <img src="https://picsum.photos/300/300?e"/>
    <img class= "rounded-br-xl" src="https://picsum.photos/300/300?f"/>
</div>
</template>

<style>
.photoGrid {
    display: grid;
    grid-template-columns: auto auto auto;
    grid-template-rows: 50% 50%;
    gap: 2px;
}
img {
    object-fit: cover;
    width: 100%;
    height: 100%;
}
</style>