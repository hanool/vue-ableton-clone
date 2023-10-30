<template>
	<main>
		<header>
			<AbletonLogo />
			<FirstNav />
			<SubNav />
		</header>

		<RouterView />

	</main>
</template>

<script setup lang="ts">
import { RouterView } from 'vue-router'
import AbletonLogo from './components/AbletonLogo.vue'
import FirstNav from './components/FirstNav.vue'
import SubNav from './components/SubNav.vue'

</script>

<style scoped>
main {
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	margin: auto;
	position: relative;
}

@media screen and (min-width: 100em) {
	main {
		max-width: 100em;
	}
}

header {
	width: 100%;
}
</style>
