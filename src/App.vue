<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import MainIcon from './components/MainIcon.vue'
</script>

<template>
	<header>
		<nav class="first-nav">
			<RouterLink to="/live">
				<a class="logo">
					<MainIcon />
				</a>
			</RouterLink>
			<div class="w-100">
				<ul>
					<li class="first-item">
						<RouterLink to="/live">Live</RouterLink>
					</li>
					<li>
						<RouterLink to="/push">Push</RouterLink>
					</li>
					<li>
						<RouterLink to="/note">Note</RouterLink>
					</li>
					<li>
						<RouterLink to="/link">Link</RouterLink>
					</li>
					<li>
						<RouterLink to="/shop">Shop</RouterLink>
					</li>
					<li>
						<RouterLink to="/packs">Packs</RouterLink>
					</li>
					<li>
						<RouterLink to="/help">Help</RouterLink>
					</li>
					<li>
						<RouterLink to="/more">More +</RouterLink>
					</li>

					<li class="seperate-to-right">
						<RouterLink to="/try">Try Live for free</RouterLink>
					</li>
					<li>
						<RouterLink to="/register">Log in or register</RouterLink>
					</li>
				</ul>
			</div>
		</nav>
		<div class="main-nav-seperator"></div>
		<nav>
			<RouterLink to="/about">About</RouterLink>
			<RouterLink to="/jobs">Jobs</RouterLink>
			<RouterLink to="/apprenticeships">Apprenticeships</RouterLink>

		</nav>
	</header>

	<RouterView />
</template>

<style scoped>
li {
	padding: auto;
	margin: 12px;
}

.logo {
	position: absolute;
	left: 1rem;
	top: 1rem;
}

.first-nav {
	width: 100%;
	display: flex;
	flex-direction: row;
	position: relative;
}

.first-nav ul {
	display: flex;
	flex-direction: row;
}

.first-nav li {
	list-style: none;
}

.first-item {
	margin-left: 41px;
}

.seperate-to-right {
	margin-left: auto;
}

.w-100 {
	width: 100%;
}
</style>
