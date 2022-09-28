<script>
	import CustomLayout from '../components/CustomLayout.svelte';
	let currIndex = 0;
	const videoSrc = [''];
</script>

<CustomLayout largeScreen={true}>
	<!-- svelte-ignore a11y-media-has-caption -->
	<!-- <div class="flex items-center text-3xl">
        <div><i class="fa-solid fa-chevron-left p-2"></i></div>
        <div class="flex-1 uppercase text-center"><h2>title</h2></div>
        <div><i class="fa-solid fa-chevron-right p-2"></i></div>
    </div> -->
	<!-- <video class="w-full" autoplay="autoplay" muted  loop="loop" playsinline="playsinline" >
        <source src="swoldierfitness.mp4" type="video/mp4">
    </video>

    <div class="absolute inset-0 z-30 border-2 border-white border-solid"></div>

	<div class="absolute inset-0 z-30" >
        <div class="absolute top-1/2 -translate-y-1/2 left-0 shads text-5xl  text-sky-200 hover:text-sky-400 duration-150 cursor-pointer px-4"><i class="fa-solid fa-chevron-left"></i></div>
        <div class="absolute top-1/2 -translate-y-1/2 right-0 shads text-5xl text-sky-200 hover:text-sky-400 duration-150 cursor-pointer px-4"><i class="fa-solid fa-chevron-right"></i></div>
        <div class="absolute px-4 py-2 top-0 text-sm font-medium right-0 flex items-center gap-2"> <i class="fa-solid fa-circle-info text-yellow-400 duration-150 hover:text-yellow-600 cursor-pointer text-4xl"></i> </div>
    </div> -->

	<div class="flex flex-col">
		<div class="grid grid-cols-1 lg:grid-cols-2 sm:p-4 bg-slate-100">
			<a
				href="https://www.swoldierfitness.com"
				target="_blank"
				class="max-w-full shadow cursor-pointer relative group"
			>
				<video class="w-full" autoplay="autoplay" muted loop="loop" playsinline="playsinline">
					<source src="swoldierfitness.mp4" type="video/mp4" />
				</video>
				<div class="absolute inset-0 bg-black opacity-0 group-hover:opacity-10" />
			</a>
			<div class="flex flex-col sm:gap-2 justify-center items-center p-8">
				<a href="https://www.swoldierfitness.com" target="_blank" class="hover:opacity-70">
					<h2 class="text-center font-semibold text-3xl sm:text-4xl">SWOLDIER FITNESS</h2>
				</a>
				<p class="text-justify">
					Swoldier Fitness is a new generation of fitness web application that uses intelligent
					algorithms and web infrastructure to emulate personal training, but for a fraction of the
					price. The free base product serves to generate thousands of personalized & highly
					effective workouts to suit any user needs, complete with exercise descriptions and workout
					tracking. The premium product offers training analytics, training programs, at-home
					friendly workout generation, and access to the exclusive stretching, physio-therapy and
					warmup generators.
				</p>
			</div>
		</div>
		<div class="flex flex-col lg:flex-row lg:items-center lg:flex-row-reverse sm:p-4">
			<a
				href="https://famous-kashata-6dcdd0.netlify.app/"
				class="max-w-full shadow flex-1 relative group cursor-pointer"
				target="_blank"
			>
				<video class="w-full" autoplay="autoplay" muted loop="loop" playsinline="playsinline">
					<source src="roadmap.mp4" type="video/mp4" />
				</video>
				<div class="absolute inset-0 bg-black opacity-0 group-hover:opacity-10" />
			</a>
			<div class="flex flex-col sm:gap-2 flex-1 justify-center items-center p-8">
				<a
					href="https://famous-kashata-6dcdd0.netlify.app/"
					target="_blank"
					class="hover:opacity-70"
				>
					<h2 class="text-center font-semibold text-3xl sm:text-4xl">WEBDEV ROADMAP</h2>
				</a>
				<p class="text-justify">
					The Webdev Codemap is a web app that aims to amalgamate all of the top, free, online
					learning resources for self-teaching web development. It structures said resources into a
					fun and interactive roadmap that provides the user with a more personal and engaging
					learning experience as they work through the content. Local storage is used to personalize
					the experience and store the users progression.
				</p>
			</div>
		</div>
		<div class="grid grid-cols-1 lg:grid-cols-2 sm:p-4 bg-slate-100">
			<a
				href="https://galactiplanner.com"
				target="_blank"
				class="max-w-full shadow relative group cursor-pointer"
			>
				<video class="w-full" autoplay="autoplay" muted loop="loop" playsinline="playsinline">
					<source src="galactiplanner.mp4" type="video/mp4" />
				</video>
				<div class="absolute inset-0 bg-black opacity-0 group-hover:opacity-10" />
			</a>
			<div class="flex flex-col sm:gap-2 justify-center items-center p-8">
				<a href="https://galactiplanner.com" target="_blank" class="hover:opacity-70">
					<h2 class="text-center font-semibold text-3xl sm:text-4xl">GALACTIPLANNER</h2>
				</a>
				<p class="text-justify">
					Galactiplanner is an organizational web application that allows the user to better
					compartmentalize their life. Giving the user the ability to fill out their planner with
					Goals, Notes & Reminders, each with a unique informational structure. The planner is
					responsive and the authentication and database infrastructure allows the user to take the
					planner with them on their mobile, and then access it later on a different device.
				</p>
			</div>
		</div>
	</div>
</CustomLayout>

<style>
	video {
		max-width: 100%;
		object-fit: contain;
	}

	/* i {
        color: #465e75;

    } */
</style>
