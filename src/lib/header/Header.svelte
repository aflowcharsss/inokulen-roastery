<script>
	import { page } from '$app/stores';
</script>

<header class="text-xs uppercase font-medium tracking-wider text-gray-800">
	<!-- Top Nav -->
	<div class="top py-4 border-b border-b-1 border-gray-800">
		<ul class="flex items-center justify-between">
			<div class="left flex items-center space-x-6">
				<li class:active={$page.url.pathname === '/'} class="flex items-center space-x-2">
					<svg
						class="h-6 w-6"
						xmlns="http://www.w3.org/2000/svg"
						fill="#1f2937"
						viewBox="0 0 256 256"
						><rect width="256" height="256" fill="none" /><line
							x1="40"
							y1="128"
							x2="216"
							y2="128"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/><line
							x1="40"
							y1="64"
							x2="216"
							y2="64"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/><line
							x1="40"
							y1="192"
							x2="216"
							y2="192"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/></svg
					>
					<a sveltekit:prefetch href="/">Menu</a>
				</li>
				<li class:active={$page.url.pathname === '/'} class="flex items-center space-x-2">
					<svg
						class="w-5 h-5"
						xmlns="http://www.w3.org/2000/svg"
						fill="#1f2937"
						viewBox="0 0 256 256"
						><rect width="256" height="256" fill="none" /><circle
							cx="116"
							cy="116"
							r="84"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/><line
							x1="175.4"
							y1="175.4"
							x2="224"
							y2="224"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/></svg
					>
					<a sveltekit:prefetch href="/">Pencarian</a>
				</li>
			</div>
			<div class="center">
				<a href="https://kit.svelte.dev">
					<img class="w-20 h-20 object-cover" src="/static/logo-nav.png" alt="SvelteKit" />
				</a>
			</div>
			<div class="right flex items-center space-x-6">
				<li class:active={$page.url.pathname === '/'} class="flex items-center space-x-2">
					<svg
						class="w-5 h-5"
						xmlns="http://www.w3.org/2000/svg"
						fill="#1f2937"
						viewBox="0 0 256 256"
						><rect width="256" height="256" fill="none" /><path
							d="M208.8,72H47.2a8.1,8.1,0,0,0-8,7.1L25,207.1a8,8,0,0,0,7.9,8.9H223.1a8,8,0,0,0,7.9-8.9l-14.2-128A8.1,8.1,0,0,0,208.8,72Z"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/><path
							d="M88,104V72a40,40,0,0,1,80,0v32"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/></svg
					>
					<a sveltekit:prefetch href="/">Keranjang</a>
				</li>
				<li class:active={$page.url.pathname === '/'} class="flex items-center space-x-2">
					<svg
						class="w-5 h-5"
						xmlns="http://www.w3.org/2000/svg"
						fill="#1f2937"
						viewBox="0 0 256 256"
						><rect width="256" height="256" fill="none" /><circle
							cx="128"
							cy="96"
							r="64"
							fill="none"
							stroke="#1f2937"
							stroke-miterlimit="10"
							stroke-width="16"
						/><path
							d="M31,216a112,112,0,0,1,194,0"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/></svg
					>
					<a sveltekit:prefetch href="/">Akun</a>
				</li>
			</div>
		</ul>
	</div>

	<!-- Bottom Nav -->
	<nav class="bottom py-4 border-b border-b-1 border-gray-800">
		<!-- <svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg> -->
		<ul class="flex items-center justify-center space-x-16">
			<li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/">Rumah</a></li>
			<li class:active={$page.url.pathname === '/about'}>
				<a sveltekit:prefetch href="/about">Biji Pilihan</a>
			</li>
			<li class:active={$page.url.pathname === '/todos'}>
				<a sveltekit:prefetch href="/todos">Menu Kopi</a>
			</li>
			<li class:active={$page.url.pathname === '/todos'}>
				<a sveltekit:prefetch href="/todos">Cerita Petani</a>
			</li>
			<li class:active={$page.url.pathname === '/todos'}>
				<a sveltekit:prefetch href="/todos">Kontak Aja</a>
			</li>
			<li class:active={$page.url.pathname === '/todos'}>
				<a sveltekit:prefetch href="/todos">Tentang Kami</a>
			</li>
		</ul>
		<!-- <svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg> -->
	</nav>

	<div class="corner">
		<!-- TODO put something else here? github link? -->
	</div>
</header>

<style>
</style>
