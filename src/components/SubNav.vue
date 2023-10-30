<template>
	<nav>
		<ul>
			<li v-for="item in subNavItems" :key="item.link">
				<RouterLink :to="item.link" :class="item.class">{{ item.label }}</RouterLink>
			</li>
		</ul>
	</nav>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'

const subNavItems = [
	{ label: "About", link: "/about", class: ["orange"] },
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
	padding: 0px;
}

li {
	list-style: none;
	margin-left: 41px;
}

li:first-child {
	margin-left: 10px;
}
</style>
