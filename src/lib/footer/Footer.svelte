<script>
	import { page } from '$app/stores';
</script>

<footer class="footer my-6 border-y border-y-1 border-gray-800">
	<div class="wrapper py-8 flex flex-col items-center justify-center border-gray-800">
		<div class="logo-footer mb-4">
			<img class="w-20 h-20 object-cover" src="./images/logo-footer.png" alt="Inokulen Logo" />
		</div>
		<div class="heading mb-6">
			<h3 class="uppercase font-extrabold text-lg tracking-wider font-mont">Inokulen Roastery</h3>
		</div>
		<div class="menu mb-12">
			<ul
				class="flex items-center justify-center space-x-16 text-xs uppercase font-medium tracking-wider"
			>
				<li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/">Rumah</a></li>
				<li class:active={$page.url.pathname === '/about'}>
					<a sveltekit:prefetch href="/about">Biji Pilihan</a>
				</li>
				<li class:active={$page.url.pathname === '/about'}>
					<a sveltekit:prefetch href="/about">Menu Kopi</a>
				</li>
				<li class:active={$page.url.pathname === '/about'}>
					<a sveltekit:prefetch href="/about">Cerita Petani</a>
				</li>
				<li class:active={$page.url.pathname === '/about'}>
					<a sveltekit:prefetch href="/about">Kontak Aja</a>
				</li>
				<li class:active={$page.url.pathname === '/about'}>
					<a sveltekit:prefetch href="/about">Tentang Kami</a>
				</li>
			</ul>
		</div>
		<div class="copyright text-xs font-medium tracking-wider">
			&copy; Copyright Inokulen Roastery 2022 &minus; All Right Reserverd
		</div>
	</div>
</footer>
