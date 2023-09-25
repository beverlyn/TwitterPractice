<script setup lang="ts">
import { ref } from "vue";
import { vOnClickOutside } from '@vueuse/components'
import type { OnClickOutsideHandler } from '@vueuse/core'
import MoreMenu from "./components/MoreMenu.vue";

const showMenu = ref(false);
const toggleNav = () => (showMenu.value = !showMenu.value);
const dropdownHandler: OnClickOutsideHandler = (event) => {
  console.log(event)
  showMenu.value = false
}

</script>

<template>
<div
    class="
    text-[20px]
    h-screen
    w-[250px]
    flex
    flex-col
    justify-between
    ">

    <div>
        <div class="
            h-[56px]
            flex
            items-center
        ">
            <IconMingcuteFlower2Line 
                class="
                text-[40px]
                rounded-full
                p-[4px]
                hover:bg-neutral-900
            "/>
        </div>

        <div class="relative">
            <div
                class="
                grid
                grid-cols-1
                gap-[8px]"
            >
                <button class="sideMenu">
                    <IconMingcuteHome5Line/>
                    <span>
                        Home
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteSearch2Fill/>
                    <span>
                        Explore
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteNotificationLine/>
                    <span>
                        Notifications
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteMailLine/>
                    <span>
                        Messages
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteDocumentLine/>
                    <span>
                        Lists
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteBookmarkLine/>
                    <span>
                        Bookmarks
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteGroupLine/>
                    <span>
                        Communities
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteXrpLine/>
                    <span>
                        Verified
                    </span>
                </button>
                <button class="sideMenu">
                    <IconMingcuteUser2Line/>
                    <span>
                        Profile
                    </span>
                </button>
                <button class="sideMenu" @click.stop="toggleNav" >
                    <IconMingcuteMore3Line/>
                    <span>
                        More
                    </span>
                </button>
            </div>

            <div 
                :class="showMenu ? 'contents' : 'hidden'" 
                class="absolute bottom-[20px]"
                v-on-click-outside.bubble="dropdownHandler">
                <MoreMenu/>
            </div>
        </div>

        <button 
            class="
            mt-[24px]
            p-[12px]
            w-[230px]
            rounded-full
            bg-sky-600
            text-[18px]
            font-bold
            hover:bg-sky-700
        ">
            Post
        </button>
    </div>

    <button 
        class="
        rounded-full
        p-[8px]
        w-[240px]
        flex
        justify-between
        items-center
        hover:bg-neutral-900
    ">
        <div class="
            flex
            gap-[12px]
            items-center
        ">
            <img 
                src="https://picsum.photos/200/200" 
                class="
                rounded-full
                object-cover
                h-[40px]
                w-[40px]
            "/>
            <div class="text-[16px]">
                <span class="font-bold">Beverly N</span>
                <br>
                <span>
                    @beverlyn
                </span>
            </div>
        </div>

        <IconMingcuteMore1Line/>
    </button>
</div>
</template>

<style>

.sideMenu {
    background-color: black;
    padding: 8px;
    padding-right: 32px;
    border-radius: 9999px;
    display: flex;
    width: fit-content;
    gap: 24px;
    align-items: center;
    text-align: left;
}

.sideMenu:hover {
    background-color: rgb(23 23 23);
}

</style>
