<template>
	<header>
		<AbletonLogo />
		<FirstNav />
		<SubNav />
	</header>

	<RouterView />
</template>

<script setup lang="ts">
import { RouterView } from 'vue-router'
import AbletonLogo from './components/AbletonLogo.vue'
import FirstNav from './components/FirstNav.vue'
import SubNav from './components/SubNav.vue'

</script>
