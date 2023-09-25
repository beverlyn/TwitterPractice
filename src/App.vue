<script setup lang="ts">
import TwitterMenu from './TwitterMenu.vue';
import TwitterCenter from './TwitterCenter.vue';
import TwitterRight from './TwitterRight.vue';

</script>

<template>
<div class="mainPage divide-x divide-neutral-700">
	<TwitterMenu class="sticky top-0"/>
	<TwitterCenter/>
	<TwitterRight class="pl-[20px]"/>
</div>
</template>

<style>
.mainPage {
	margin: 0px;
	display: grid;
	grid-template-columns: 250px 600px 350px;
	justify-content: center;
}
</style>
