<template>
	<div class="flex-grow leading-relaxed mt-18 mb-6">
		<!-- First section -->
		<div class="flex text-md">
			<div class="my-6 md:flex block mx-auto items-center">
				<div class="text-4xl font-bold">
					<p>Full-stack web developer</p>
					<p class="text-blue">Welcome to my website</p>
				</div>
				<img class="md:h-64 h-48 mx-auto" src="../assets/web_developer.svg" alt="Hero" />
			</div>
		</div>

		<!-- Second section -->
		<div class="mx-28">
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
					class="h-40 md:h-48 md:ml-16 mx-auto"
					src="../assets/tailwind_css.svg"
					alt="Img"
				/>
			</div>
		</div>

		<!-- Projects section -->
		<div class="border-b border-t border-gray-500 mx-28">
			<!-- Title -->
			<h2 class="font-bold mb-6">Here some projects I've worked on:</h2>

			<!-- List of projects -->
			<ul class="text-blue">
				<li v-for="item in projects" :key="item.id" class="flex mb-6 items-center">
					<svg
						class="fill-current"
						width="20"
						height="20"
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
	</div>
</template>

<script>
export default {
	data() {
		return {
			projects: [
				{
					project: 'Laravel Ecommerce application tutorial on YOutube Github LInk here',
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
