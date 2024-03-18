<script setup>
import { RouterView } from 'vue-router';
import sidebar from './components/sidebar.vue';
</script>

<template>
 <div class="app">
		<!-- Sidebar -->
		<sidebar />

		<!-- Content -->
		<router-view />
	</div>
</template>
<style lang="scss">
:root {
	--primary: #ffffff;
	--primary-alt: #22c55e;
	--grey: #334155;
	--dark: #5CCAED;
	--dark-alt: #acacac;
	--light: #ffffff;
	--blue-pri: #5CCAED;
	--sidebar-width: 200px;
}

* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Fira sans', sans-serif;
}

body {
	background: var(--light);
}

button {
	cursor: pointer;
	appearance: none;
	border: none;
	outline: none;
	background: none;
}

.app {
	display: flex;

	main {
		flex: 1 1 0;
		padding: 2rem;

		@media (max-width: 1024px) {
			padding-left: 6rem;
		}
	}
}
</style>