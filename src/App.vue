<template>
	<div class="font-sans tracking-wider text-gray-800 flex flex-col h-screen" id="app">
		<Header />
		<div class="flex-grow bg-purple-300 text-lg leading-relaxed">
			Lorem ipsum dolor sit amet consectetur, adipisicing elit. Facere iste sapiente
			iusto, perspiciatis recusandae libero corporis illo inventore suscipit dolor quos
			ipsum sed laudantium sunt minus eveniet quisquam tenetur impedit fuga quaerat,
			facilis dicta. Error, voluptates cupiditate iste culpa dolores alias recusandae
			sapiente enim architecto consequuntur aliquam cum qui excepturi illum esse vitae
			eius amet nam eveniet. Culpa molestias aliquid aspernatur blanditiis. Eaque,
			adipisci nam libero praesentium omnis sint ea accusantium doloremque recusandae a
			assumenda non repudiandae soluta iusto ullam est tenetur minus? Perspiciatis
			voluptates reprehenderit aperiam, rerum quisquam ab necessitatibus similique! Magnam
			eveniet excepturi dolor harum sit sed alias?
		</div>
		<Footer />
	</div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';

export default {
	name: 'App',
	components: {
		Header,
		Footer,
	},
};
</script>

<style src="./assets/tailwind.css"></style>
