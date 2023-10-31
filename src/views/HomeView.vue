<template>
	<div class="page">
		<header>
			<MainHeaderSVG class="main-header-svg" />
		</header>
		<AboutText>
			<h1>We make
				<a href="/en/live/" class="blue">Live</a>,
				<a href="/en/push/" class="blue">Push</a> and
				<a href="/en/link/" class="blue">Link</a> — unique
				software and hardware for music creation and performance. With these products, our community of users creates
				amazing things.
			</h1>
			<p>
				Ableton was founded in 1999 and released the first version of Live in 2001. Our products are used by a community
				of
				dedicated musicians, sound designers, and artists from across the world.
			</p>
		</AboutText>
		<AboutProduct />
	</div>
</template>

<script setup lang="ts">
import MainHeaderSVG from '@/components/header/MainHeaderSVG.vue'
import AboutText from '@/components/AboutText.vue'
import AboutProduct from '@/components/AboutProduct.vue'
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
