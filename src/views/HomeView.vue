<template>
	<main>
		<div>
			<header class="main-header">
				<MainHeaderSVG class="main-header-svg" />
			</header>
		</div>
	</main>
</template>

<script setup lang="ts">
import MainHeaderSVG from '@/components/header/MainHeaderSVG.vue'
</script>

<style scoped>
.main-header {
	margin: auto;
	width: 80%;
	min-height: 500px;
	background-image: url('@/assets/header.jpg');
	background-position: 50% 50%;
	background-repeat: no-repeat;
}

header {
	display: flex;
	align-items: center;
	justify-content: center;
}
</style>
