<template>
	<nav>
		<ul>
			<li v-for="item in subNavItems" :key="item.link">
				<RouterLink :to="item.link">{{ item.label }}</RouterLink>
			</li>
		</ul>
	</nav>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'

const subNavItems = [
	{ label: "About", link: "/about" },
	{ label: "Jobs", link: "/jobs" },
	{ label: "Apprenticeships", link: "/apprenticeships" },
]
</script>

<style scoped>
nav {
	width: 100%;
	display: flex;
	flex-direction: row;
	position: relative;
}

ul {
	display: flex;
	flex-direction: row;
}

li {
	list-style: none;
	margin-left: 41px;
}
</style>
