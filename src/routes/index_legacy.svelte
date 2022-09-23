<script>
	import { onMount } from 'svelte';

	onMount(() => {
		loadHighResImage(document.getElementById('bg-img'), 'bg2.avif');
	});

	function loadHighResImage(elem, highResUrl) {
		let image = new Image();
		image.addEventListener('load', () => (elem.src = highResUrl));
		image.src = highResUrl;
	}
</script>

<main
	class="flex-1 p-4 sm:p-7 relative text-xs sm:text-sm flex justify-center items-center z-10 flex-col text-white"
>
	<h1 class="font-extrabold uppercase text-3xl sm:text-5xl md:text-6xl">James McArthur</h1>
	<h2 class="text-sm sm:text-base text-white">Design, Code & Everything in Between</h2>
	<ul class="relative w-[230px] sm:w-[300px] max-w-full aspect-square ">
		<li class="menu-item">
			<a href="/resume">
				<i
					class="fa-solid fa-user-astronaut relative after:absolute after:top-full after:content-['Resume'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2"
				/>
				<div class="" />
			</a>
			<!-- <span>Resume</span> -->
			<!-- <div>Resume</div> -->
		</li>
		<li class="menu-item">
			<a href="/projects">
				<i
					class="fa-solid fa-flask  after:absolute after:top-full after:content-['Projects'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2"
				/>
				<div class="" />
			</a>
			<!-- <span>Projects</span> -->

			<!-- <div>Projects</div> -->
		</li>
		<li class="menu-item">
			<a href="https://www.youtube.com/c/Smoljames" target="_blank">
				<i
					class="fa-brands fa-youtube  after:absolute after:top-full after:content-['Youtube'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2"
				/>
				<div class="" />
			</a>
			<!-- <span>Youtube</span> -->
			<!-- <div>Youtube</div> -->
		</li>
		<li class="menu-item">
			<!-- <div>Medium</div> -->
			<a href="https://medium.com/@_Smoljames" target="_blank">
				<i
					class="fa-brands fa-medium  after:absolute after:top-full after:content-['Blog'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2"
				/>
				<div class="" />
			</a>
			<!-- <span>Blog</span> -->
		</li>
		<li class="menu-item">
			<a href="https://github.com/jamezmca" target="_blank">
				<!-- <div>Github</div> -->
				<i
					class="fa-brands fa-github  after:absolute after:top-full after:content-['Github'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2 "
				/>
				<div class="" />
			</a>
			<!-- <span>Github</span> -->
		</li>
		<li class="menu-item">
			<!-- <div>LinkedIn</div> -->
			<a href="https://www.linkedin.com/in/jamezmcarthur/" target="_blank">
				<i
					class="fa-brands fa-linkedin  after:absolute after:top-full after:content-['LinkedIn'] after:text-xs after:left-1/2 after:opacity-0 hover:after:opacity-100 after:duration-300 after:-translate-x-1/2"
				/>
				<div class="" />
			</a>
			<!-- <span>LinkedIn</span> -->
		</li>
	</ul>
</main>

<div class="absolute inset-0 z-0">
	<img id="bg-img" class="object-cover w-full h-full z-10" src="bg2-lowres.jpeg" alt="bg-img" />
	<!-- <img class="object-cover w-full h-full z-[1]" src="bg2-lowres.jpeg" alt="bg-img"/> -->
</div>

<style>
	h1,
	h2 {
		text-shadow: 0 0 1px transparent, 0 1px 2px rgb(0 0 0 / 50%);
	}

	.menu-item {
		position: absolute;
		display: grid;
		place-items: center;
		top: 0;
		bottom: 0;
		left: 0;
		right: 0;
		margin: auto;
		height: fit-content;
		width: fit-content;
		/* background: yellow; */
		transform-origin: center;
		cursor: pointer;
	}

	.menu-item i::after {
		font-family: 'Poppins', sans-serif;
		text-transform: uppercase;
		font-weight: 500;
	}

	/* .menu-item span {
		position: absolute;
		top: 100%;
		left: 50%;
		transform: translateX(-50%);
	} */

	/* .menu-item:hover i {
		opacity: 0.5;
	} */

	.menu-item i {
		font-size: 1.9rem;
		position: relative;
		z-index: 20;
	}

	.menu-item div {
		position: absolute;
		inset: 0;
		background: black;
		filter: blur(40px);
		opacity: 0.4;
		/* z-index: 20; */
	}

	.menu-item:nth-child(1) {
		transform: rotate(60deg) translateX(-70px);
	}
	.menu-item:nth-child(2) {
		transform: rotate(120deg) translateX(-70px);
	}
	.menu-item:nth-child(3) {
		transform: rotate(180deg) translateX(-70px);
	}
	.menu-item:nth-child(4) {
		transform: rotate(240deg) translateX(-70px);
	}
	.menu-item:nth-child(5) {
		transform: rotate(300deg) translateX(-70px);
	}
	.menu-item:nth-child(6) {
		transform: rotate(360deg) translateX(-70px);
	}

	.menu-item:nth-child(1) i {
		transform: rotate(-60deg);
	}
	.menu-item:nth-child(2) i {
		transform: rotate(-120deg);
	}
	.menu-item:nth-child(3) i {
		transform: rotate(-180deg);
	}
	.menu-item:nth-child(4) i {
		transform: rotate(-240deg);
	}
	.menu-item:nth-child(5) i {
		transform: rotate(-300deg);
	}
	.menu-item:nth-child(6) i {
		transform: rotate(-360deg);
	}

	@media (min-width: 640px) {
		.menu-item i {
			font-size: 2.5rem;
		}

		.menu-item:nth-child(1) {
			transform: rotate(60deg) translateX(-90px);
		}
		.menu-item:nth-child(2) {
			transform: rotate(120deg) translateX(-90px);
		}
		.menu-item:nth-child(3) {
			transform: rotate(180deg) translateX(-90px);
		}
		.menu-item:nth-child(4) {
			transform: rotate(240deg) translateX(-90px);
		}
		.menu-item:nth-child(5) {
			transform: rotate(300deg) translateX(-90px);
		}
		.menu-item:nth-child(6) {
			transform: rotate(360deg) translateX(-90px);
		}
	}
</style>
