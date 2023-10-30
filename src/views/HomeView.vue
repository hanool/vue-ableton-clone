<template>
	<div class="page">
		<header>
			<MainHeaderSVG class="main-header-svg" />
		</header>
	</div>
</template>

<script setup lang="ts">
import MainHeaderSVG from '@/components/header/MainHeaderSVG.vue'
</script>

<style scoped>
@media screen and (min-width: 100em) {
	.page {
		width: 1600px;
	}
}

header {
	display: block;
	background-image: url('@/assets/header.jpg');
	background-position: 50% 50%;
	background-repeat: no-repeat;
	background-size: cover;
	display: flex;
	align-items: center;
	justify-content: center;
	min-height: calc(100vh - 120px);
	margin: 0px 133px;
}
</style>
