<script setup lang="ts">
import { faker } from '@faker-js/faker';
defineProps({
    imageUrl: String,
})

const randomText = faker.lorem.lines()
</script>

<template>
<div class="
    post
    w-[600px]
    px-[16px]
    py-[8px]
">
    <img src="https://picsum.photos/200/200"
        class="w-[40px] h-[40px] rounded-md"/>
    <div>
        <div class="
            flex
            flex-cols
            justify-between
            leading-tight
        ">
            <span class="self-start">
                <span class="hover:underline">
                    Beverly N
                </span>
                <span class="text-gray-500">
                    @beverlyn
                </span>
                <span class="text-gray-500">
                    • 1hr
                </span>
            </span>
            <span class="p-[6px] rounded-full hover:bg-sky-600/40">
                <IconMingcuteMore1Line 
                class="
                text-gray-500
                hover:text-sky-600"
            />
            </span>
        </div>

        <span>
            {{ randomText }}
        </span>

        <img 
            class="w-full h-auto rounded-2xl my-[16px]"
            :src="imageUrl"/>

        <div class="
            text-gray-500
            text-[14px]
            flex
            justify-between
        ">
            <button class="actionButtons hover:text-sky-600">
                <span class="p-[6px] rounded-full hover:bg-sky-600/40">
                    <IconIconamoonComment />
                </span>
                5
            </button>
            <span class="actionButtons hover:text-green-600">
                <span class="p-[6px] rounded-full hover:bg-green-600/40">
                    <IconFa6SolidRetweet />
                </span>
                145
            </span>
            <span class="actionButtons hover:text-rose-600">
                <span class="p-[6px] rounded-full hover:bg-rose-600/40">
                    <IconMingcuteHeartLine />
                </span>
                1,539
            </span>
            <span class="actionButtons hover:text-sky-600">
                <span class="p-[6px] rounded-full hover:bg-sky-600/40">
                    <IconIonMdStats/>
                </span>
                1.2M
            </span>  
            <span class="actionButtons hover:text-sky-600">
                <span class="p-[6px] rounded-full hover:bg-sky-600/40">
                    <IconIconamoonShare2Fill/>
                </span>
            </span>
        </div>
    </div>
</div>
</template>

<style>
.post {
    display: grid;
    grid-template-columns: 40px 520px;
    gap: 8px;
}
.actionButtons {
    display: flex;
    gap: 4px;
    align-items: center;
}
</style>
