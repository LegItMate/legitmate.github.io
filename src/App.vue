<script setup>
</script>

<template>
	<div class="home">
		<nav class="navbar">
			<a>Home</a>
			<a>About</a>
		</nav>
		<div class="main">
			<img alt="pfp" class="logo" src="./assets/pfp.png" />
			<div class="socials">
				<a href="https://github.com/LegItMate" class="social" target="_blank">
					<img src="./assets/github.svg" />
					<span>LegItMate</span>
				</a>
				<a href="https://discord.com/app" class="social" target="_blank">
					<img src="./assets/discord.svg" />
					<span>LegItMate#6667</span>
				</a>
				<a href="https://twitter.com/" class="social" target="_blank">
					<img src="./assets/twitter.svg" />
					<span>Soon</span>
				</a>
			</div>
		</div>
	</div>
</template>

<style scoped>
.home {
	height: 100%;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: space-between;
}

@media (min-width: 1024px) {
	.home {
		height: 65%;
	}

	.social:hover span {
		opacity: 1;
		width: 180px;
	}
}

@media (min-height: 900px) {
	.home {
		height: 50%;
	}
	.social span {
		opacity: 1 !important;
	}
}

.logo {
	width: 175px;
	height: 175px;
	border-radius: 50%;
	margin-right: 30px;
}

.navbar {
	display: flex;
	align-items: center;
	justify-content: center;
	font-size: 1.1rem;
	margin-top: 2rem;
}

.navbar a.router-link-exact-active {
	background-color: transparent;
}

.navbar a:not(.router-link-exact-active):hover {
	color: hsla(160, 100%, 37%, 1);
}

.navbar a {
	padding: 0 1rem;
	color: var(--color-text);
}

.navbar a:not(:last-of-type) {
	border-right: 1px solid var(--color-border);
}

.main {
	display: flex;
	flex-direction: row;
}

.socials {
	margin-top: 15px;
	height: 150px;
	justify-content: space-evenly;
	min-width: 40px;
	max-width: 180px;
	padding-left: 30px;
	display: flex;
	flex-direction: column;
	border-left: 1px solid var(--color-border);
}

.social {
	display: flex;
	flex-direction: row;
	min-width: 50px;
	margin-bottom: 5px;
	text-decoration: none;
	color: var(--color-text);
}

.social span {
	margin-left: 15px;
	margin-top: 4px;
	display: flex;
	opacity: 0;
	font-size: 16px;
	font-weight: 500;
}

.social img {
	height: 30px;
	width: 30px;
}
</style>
