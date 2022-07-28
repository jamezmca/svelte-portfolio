<div class=" flex flex-col min-h-screen text-xs sm:text-sm">
	<header class="border-b border-solid border-slate-200">
		<h1 class="max-w-[1000px] w-full mx-auto p-4 sm:p-7  font-semibold text-md uppercase">
			<a href="/" class="hover:text-blue-500 cursor-pointer sm:hidden">JM</a>
			<a href="/" class="hover:text-blue-500 cursor-pointer hidden sm:inline">James McArthur</a>
		</h1>
	</header>
	<section class="flex-1 flex flex-col w-full max-w-[1000px] mx-auto p-4 sm:p-7">
		<slot />
	</section>
	<footer
		class="grid place-items-center p-10 sm:p-14 sm:gap-14 border-t border-solid border-slate-200"
	>
		<div class="flex flex-col gap-5">
            <div class="flex items-center">
                <a href='/resume'>Resume</a>
                <div class="px-3">|</div>
                <a href='/projects'>Projects</a>
                <div class="px-3">|</div>
                <a href='https://medium.com/@_Smoljames' target="_blank">Blog</a>
            </div>
			<div class="flex items-center w-fit mx-auto gap-6">
				<a href="https://www.linkedin.com/in/jamezmcarthur/" target="_blank">
					<i class="fa-brands fa-linkedin  " />
					<div class="" />
				</a>
				<a href="https://github.com/jamezmca" target="_blank">
					<!-- <div>Github</div> -->
					<i class="fa-brands fa-github  " />
					<div class="" />
				</a>
				<a href="https://www.youtube.com/c/Smoljames" target="_blank">
					<i class="fa-brands fa-youtube " />
					<div class="" />
				</a>
			</div>
		</div>
	</footer>
</div>

<style>
	h1 {
		color: #334455;
	}

    footer {
        color: #818a91;
    }

	footer i {
		font-size: 1.3rem;
	}

    footer i:hover,
    footer a:hover {
        opacity: 0.5;
    }
</style>
