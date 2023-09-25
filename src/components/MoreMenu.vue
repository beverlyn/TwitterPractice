<template>
<div class="
    moreContainer
    w-[300px]
    bg-black
    rounded-xl
    font-bold
">
    <div class="w-[300px]">
        <span class="moreMenu px-[16px] py-[8px] hover:bg-gray-700 hover:rounded-t-xl">
            <IconHumbleiconsAtSymbol/>
            <span>
                Connect
            </span>
        </span>
        <span class="moreMenu px-[16px] py-[8px] hover:bg-gray-700">
            <IconFluentMoney16Regular/>
            <span>
                Monetization
            </span>
        </span>
    </div>
    
    <div class="px-[16px]"><hr></div>
    
    <div class="text-[16px]">
        <span class="moreMenuSub px-[16px] py-[8px] hover:bg-gray-700">
            <span>
                Creator Studio
            </span>
            <IconMaterialSymbolsKeyboardArrowDown/>
        </span>
        <span class="moreMenuSub px-[16px] py-[8px] hover:bg-gray-700">
            <span>
                Professional Tools
            </span>
            <IconMaterialSymbolsKeyboardArrowDown/>
        </span>
        <span class="moreMenuSub px-[16px] py-[8px] hover:bg-gray-700 hover:rounded-b-xl">
            <span>
                Settings and Support
            </span>
            <IconMaterialSymbolsKeyboardArrowDown/>
        </span>
    </div>
</div>
</template>

<style>
.moreContainer {
    box-shadow: 0 0 10px -2px white;
}

hr {
    height: 05.px;
}
.moreMenu {
    display: flex;
    gap: 24px;
    align-items: center;
}

.moreMenuSub {
    display: flex;
    justify-content: space-between;
}
</style>