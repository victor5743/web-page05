<template>
	<div class="flex-grow leading-relaxed mt-18 mb-6">
		<!-- First section -->
		<div class="flex text-md">
			<div class="my-10 md:my-6 md:flex block mx-6 md:mx-auto items-center">
				<div class="text-4xl font-bold">
					<p>Full-stack web developer</p>
					<p class="text-blue">Welcome to my website</p>
				</div>
				<img class="md:h-64 h-48 mx-auto" src="../assets/web_developer.svg" alt="Hero" />
			</div>
		</div>

		<!-- Second section -->
		<div class="mx-6 md:mx-28">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum earum, itaque alias
			praesentium temporibus assumenda culpa animi deserunt ratione! Incidunt debitis
			culpa optio, error exercitationem placeat aliquid fugit maxime quas maiores vitae
			distinctio sit libero ut doloremque quia dolore. Non, eos nam ea ipsum obcaecati
			officiis. Sed, rem cupiditate eveniet accusantium mollitia quas dolorem, labore iste
			explicabo, culpa voluptatum ex doloremque. Accusantium dolor fugit dolores, delectus
			placeat consectetur laboriosam, perferendis fuga sed asperiores saepe quidem porro
			nihil quos ratione id commodi, quam illum repellat? Neque deserunt blanditiis vitae
			harum fugit aut quibusdam ipsum? Tenetur quidem necessitatibus repellat labore
			praesentium nobis.
		</div>

		<!-- Third section -->
		<div class="flex justify-center">
			<div class="block md:flex items-center my-8">
				<img
					class="h-40 md:h-48 md:mr-16 mb-4 md:mb-0 mx-auto"
					src="../assets/code_inspection.svg"
					alt="Img"
				/>
				<img
					class="h-40 md:h-48 md:ml-16 mx-auto hidden sm:block"
					src="../assets/tailwind_css.svg"
					alt="Img"
				/>
			</div>
		</div>

		<!-- Projects section -->
		<div class="border-b border-t border-gray-500 mx-6 md:mx-28">
			<!-- Title -->
			<h2 class="font-bold mb-6 mt-6">Here some projects I've worked on:</h2>

			<!-- List of projects -->
			<ul class="text-blue">
				<li v-for="item in projects" :key="item.id" class="flex mb-6 items-center">
					<svg
						class="fill-current h-6 w-6"
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 490.05 490.05"
					>
						<path
							d="M418.275 418.275c95.7-95.7 95.7-250.8 0-346.5s-250.8-95.7-346.5 0-95.7 250.8 0 346.5 250.9 95.7 346.5 0zm-261.1-210.7l55.1 55.1 120.7-120.6 42.7 42.7-120.6 120.6-42.8 42.7-42.7-42.7-55.1-55.1 42.7-42.7z"
						/>
					</svg>
					<a href="#" class="text-gray-800 ml-4 hover:underline hover:text-blue">
						{{ item.project }}
					</a>
				</li>
			</ul>
		</div>

		<!-- About me section -->
		<div class="mx-6 md:mx-28 my-6 border-b border-gray-500">
			<h2 class="font-bold">About me:</h2>

			<!-- Image and text -->
			<div class="block md:flex items-center">
				<img
					class="w-20 h-20 rounded-full mx-auto mb-4"
					src="../assets/man.svg"
					alt="User"
				/>
				<p class="md:ml-4">
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem libero
					temporibus impedit quo consectetur, culpa delectus autem? Quaerat magnam sunt
					delectus incidunt, ex qui esse accusamus provident modi, ad suscipit
				</p>
			</div>

			<!-- Youtube video -->
			<iframe
				class="w-auto h-auto md:h-64 md:w-128 mb-6 mx-auto"
				src="https://www.youtube.com/embed/uHo6o1TNQeE"
				frameborder="0"
				allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
				allowfullscreen
			></iframe>
		</div>

		<!-- Contact section -->
		<div class="border-b border-gray-500 mx-6 md:mx-28 my-6">
			<h2 class="font-bold mb-6">Contact me:</h2>
			<p class="mb-6">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, natus?
				Necessitatibus, magnam consectetur, aliquid animi saepe sit voluptatum velit eum
				expedita officia deleniti. Exercitationem laborum sit alias aperiam aliquam earum!
			</p>
		</div>

		<!-- Subscription section -->
		<div class="bg-blue-light py-6 mx-6 md:mx-28 texture">
			<!-- Text -->
			<h2 class="font-bold mb-6 text-center">Join my Newsletter</h2>
			<p class="text-center">
				Lorem ipsum dolor sit amet consectetur, adipisicing elit. Praesentium, fuga
				sapiente corrupti doloremque, rerum sunt in qui fugit quos illo ipsam cumque
				obcaecati.
			</p>

			<!-- Input -->
			<form action="#">
				<div class="my-4 block md:flex mx-6 md:mx-28 md:justify-center">
					<div class="flex justify-center">
						<input
							class="sm:flex-1 text-gray-400 px-4 py-2 rounded-md shadow-md outline-none border md:rounded-r-none focus:border-blue"
							name="email"
							type="email"
							placeholder="Enter your email"
							required
						/>
					</div>

					<div class="flex justify-center">
						<button
							class="bg-blue hover:bg-blue-dark text-white rounded-md md:rounded-l-none px-4 py-2 focus:outline-none uppercase mt-4 md:mt-0"
						>
							Suscribe
						</button>
					</div>
				</div>
			</form>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			projects: [
				{
					project: 'Laravel Ecommerce application tutorial on Youtube Github LInk here',
				},
				{
					project: 'Home Value Inc. Some stuff about it there. Link here.',
				},
				{
					project: 'Here are some projects Ive worked on:',
				},
				{
					project: 'Traditional resume in HTML format. PDF format here.',
				},
			],
		};
	},
};
</script>
