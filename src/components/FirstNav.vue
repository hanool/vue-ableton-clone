<template>
	<nav>
		<div class="w-100">
			<ul>
				<li v-for="item in navItems" :key="item.label">
					<RouterLink :to="item.link" :class="item.class">{{ item.label }}</RouterLink>
				</li>
				<li class="seperate-to-right">
					<RouterLink to="/try" class="blue">Try Live for free</RouterLink>
				</li>
				<li>
					<RouterLink to="/register">Log in or register</RouterLink>
				</li>
			</ul>
		</div>
	</nav>
	<hr />
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'

const navItems = [
	{ label: "Live", link: "/live" },
	{ label: "Push", link: "/push" },
	{ label: "Note", link: "/note" },
	{ label: "Link", link: "/link" },
	{ label: "Shop", link: "/shop" },
	{ label: "Packs", link: "/packs" },
	{ label: "Help", link: "/help" },
	{ label: "More +", link: "/more", class: ["orange"] },
]
</script>

<style scoped>
.seperate-to-right {
	margin-left: auto;
}

.w-100 {
	width: 100%;
}

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
	padding: auto;
	list-style: none;
	margin-left: 41px;
}
</style>
