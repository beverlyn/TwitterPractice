<script setup lang="ts">
import Post from './components/Post.vue';
</script>

<template>
<div class="
    w-[600px]
">
    <div 
        class="
        header
        fixed
        w-[600px]
        h-[56px]
        top-0
        bg-black/60
        backdrop-blur-md
        z-[9999]
        px-[16px]
    ">
        <IconMaterialSymbolsArrowLeftAlt 
            class="
                self-center
                text-[28px]
                hover:bg-neutral-900
                rounded-full
                p-[4px]
        "/>
        <div class="text-left my-auto">
            <p class="
                text-[20px]
                font-bold
            ">
                Beverly N
            </p>
            <p class="
                text-[12px]
                text-neutral-500
            ">
                2.23K posts
            </p>
        </div>
    </div>

    <div 
        class="
            relative
    ">

        <img 
            class="
                relative
                h-[200px]
                mt-[56px]"
            src="https://picsum.photos/600/200">

		<div class="
            absolute
			w-[140px]
			h-[140px]
            bottom-[-70px]
            left-[16px]
		">
        <img 
            class="
            rounded-full
            outline
            outline-[4px]
            outline-black"
            src="https://picsum.photos/200/200"/>
		</div>
    </div>

    <div class="
        mx-[16px]
        relative
        text-[16px]"
    >
        <span class="
            absolute 
            right-0 
            flex
            gap-[8px]
            leading-none
            mt-[16px]
        ">
            <span class="p-[8px] rounded-full border-[.5px] hover:bg-white/10">
                <IconMingcuteMore1Line/>
            </span>
            <span class="p-[8px] rounded-full border-[.5px] hover:bg-white/10">
                <IconMaterialSymbolsNotificationAddOutline/>
            </span>
            <button 
                class="
                font-bold
                w-[116px] 
                py-[8px] 
                px-[16px] 
                rounded-full 
                border-[.5px] 
                hover:before:content-['Unfollow']
                hover:text-red-500
                hover:border-red-500
                hover:bg-red-500/10"
            >
                <span class="following">Following</span>
            </button>
        </span>
    </div>

    <div class="
            mt-[88px]
            px-[16px]
    ">
        <p class="
                text-[20px]
                font-bold
            ">
            Beverly N
        </p>
        <p class="
            text-[16px]
            text-neutral-500
            mb-[12px]
        ">
            @beverlyn
        </p>
		<p>
			Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
		</p>
        <div class="text-neutral-500 my-[8px]">
            <span>
                <IconPhMapPin class="inline"/>
                Tokyo, JP
            </span>

            <span class="ml-[16px]">
                <IconPhLinkSimple class="inline"/>
                <a href="beverlynguyen.com"
                    class="
                    text-sky-600
                    hover:underline
                ">
                    beverlynguyen.com
                </a>
            </span>

            <span class="ml-[16px]">
                <IconMaterialSymbolsCalendarMonthOutline class="inline"/>
                Joined August 2023
            </span>
        </div>

        <div class="font-bold text-[14px] mb-[8px]">
            <span class="hover:underline">
                2.8K <span class="font-normal text-neutral-500">Following</span>
            </span>
            <span class="ml-[16px] hover:underline">
                8K <span class="font-normal text-neutral-500">Followers</span>
            </span>
        </div>

		<span class="text-[12px] text-neutral-500 mb-[32px]">
			Not followed by anyone you’re following
		</span>

        <div class="
            text-neutral-500
            flex
            justify-around
            items-stretch
            gap-0
            leading-10
            border-b-[1px] 
            border-neutral-700
            w-[599px]
            mx-[-16px]
        ">
            <button 
                class="tabs">
                Posts
            </button>
            <button class="tabs">
                Affiliates
            </button>
            <button class="tabs">
                Replies
            </button>
            <button class="tabs">
                Media
            </button>
            <button class="tabs">
                Likes
            </button>
        </div>
    </div>

    <div class="divide-y divide-neutral-700">
        <Post imageUrl="https://picsum.photos/600/600?a"/>
        <Post imageUrl="https://picsum.photos/700/300?a"/>
        <Post/>
        <Post imageUrl="https://picsum.photos/600/600?b"/>
        <Post imageUrl="https://picsum.photos/700/500?"/>
        <Post/>
    </div>
</div>
</template>

<style>
.header {
    display: grid;
    grid-template-columns: 12% 88%;
}

button:hover .following {
    display: none;
}

.tabs {
    padding: 0px 36px;
}

.tabs:hover {
    background-color: rgb(23 23 23);
}

.tabs:focus {
    text-decoration: underline;
    text-decoration-color: dodgerblue;
    text-decoration-thickness: 4px;
    text-underline-offset: 10px;
}

</style>


