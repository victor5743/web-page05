<template>
	<div
		class="font-sans tracking-wide md:tracking-wider text-gray-800 flex flex-col min-h-screen"
		id="app"
	>
		<Header />
		<Content />
		<Footer />
	</div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Content from './components/Content.vue';

export default {
	name: 'App',
	components: {
		Header,
		Footer,
		Content,
	},
};
</script>

<style src="./assets/tailwind.css"></style>
