<template>
	<RouterLink to="/live">
		<a class="logo">
			<MainIcon />
		</a>
	</RouterLink>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'
import MainIcon from './MainIcon.vue'

</script>

<style scoped>
.logo {
	position: absolute;
	left: 1rem;
	top: 1rem;
}
</style>
