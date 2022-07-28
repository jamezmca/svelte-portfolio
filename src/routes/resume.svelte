<script>
	import CustomLayout from '../components/CustomLayout.svelte';
</script>

<CustomLayout>
	<h2 class="font-bold text-4xl pb-5 pt-1">Résumé</h2>
	<h3 class="text-xl pb-5 font-semibold">James McArthur - Web Developer and Data Enthusiast</h3>
	<div class="flex flex-col gap-3 contacts">
		<div class="flex items-center gap-1.5">
			<h4>Email</h4>
			<a href="mailto:jamesmca@live.com" class="">jamesmca@live.com</a>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Github</h4>
			<a href="https://github.com/jamezmca" target="_blank" class="">jamezmca</a>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>LinkedIn</h4>
			<a href="https://www.linkedin.com/in/jamezmcarthur/" target="_blank" class="">jamezmcarthur</a
			>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Youtube</h4>
			<a href="https://www.youtube.com/c/Smoljames" target="_blank" class="">smoljames</a>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Medium</h4>
			<a href="https://medium.com/@_Smoljames" target="_blank" class="">_smoljames</a>
		</div>
	</div>
	<h3 class="text-xl py-5 font-semibold">Skills</h3>
	<div class="flex flex-col gap-3 contacts">
		<div class="flex items-center gap-1.5">
			<h4>JavaScript</h4>
			<p class="">React, React Native, SvelteKit, Node.js</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Python</h4>
			<p class="">Data analysis, Django, visualization</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Web</h4>
			<p class="">Sass, TailwindCSS, Firebase, NoSQL, SQL, AWS, and GCP</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Design</h4>
			<p class="">Canvas, Pixlr</p>
		</div>
	</div>
	<h3 class="text-xl py-5 font-semibold">Projects</h3>
	<div class="flex flex-col gap-3 contacts">
		<div class="flex items-center gap-1.5">
			<p>Checkout my latest <a href="/projects">projects</a></p>
		</div>
	</div>
	<h3 class="text-xl py-5 font-semibold">Work History</h3>
	<div class="flex flex-col gap-3 contacts">
		<div class="flex items-center gap-1.5">
			<h4>Swoldier Fitness (2022 - Present)</h4>
			<p class="">Developed an innovative fitness platform (CEO)</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Zetane Systems (2021 - Present)</h4>
			<p class="">
				Developed a Saas platform and API to facilitate machine learning robustness and QA
			</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>McMillen Jacobs Associates (2016 - 2020)</h4>
			<p class="">
				Project Engineer ensuring the successful delivery of Watercare's $1.2bn Central Interceptor
				project
			</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Maths Tutor (2013 - Present)</h4>
			<p class="">Help multitudes of students achieve their academic goals</p>
		</div>
	</div>
    <h3 class="text-xl py-5 font-semibold">Just for fun</h3>
    <div class="flex flex-col gap-3 contacts">
		<div class="flex items-center gap-1.5">
			<h4>Gym, Tennis & Running</h4>
			<p class="">Road for the Auckland Marathon & a mass monster in the gym</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Spanish Linguist</h4>
			<p class="">
				I practice my language abilities by doing my leisure reading in Spanish
			</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Backpacking</h4>
			<p class="">
				Enjoing nature on the trail
			</p>
		</div>
		<div class="flex items-center gap-1.5">
			<h4>Sunsets & Sunrises</h4>
			<p class="">Best if you can see one at least once a day</p>
		</div>
	</div>
</CustomLayout>

<style>
	.contacts div {
		position: relative;
		overflow: hidden;
		flex-wrap: wrap;
	}
	.contacts div::after {
		position: absolute;
		content: '';
		background: mediumpurple;
		height: 1.5px;
		top: calc(100% - 2px);
		right: 100%;
		/* right: 0; */
		width: 100%;
		transition-duration: 300ms;
	}

	.contacts div:hover::after {
		transform: translateX(100%);
	}

	h4 {
		font-weight: 600;
	}
	a {
		color: #1eaedb;
		/* cursor: pointer; */
	}
</style>
