<script>
	let catalogs = [
		{
			image: '/static/katalog-1.jpg',
			title: 'Kopi Sajang',
			numRate: 4.9,
			totalRate: 32,
			location: 'Sembalun, Lombok Timur',
			price: 192000
		},
		{
			image: '/static/katalog-2.jpg',
			title: 'Kopi Santong',
			numRate: 4.5,
			totalRate: 102,
			location: 'Santong, Lombok Utara',
			price: 185000
		},
		{
			image: '/static/katalog-3.jpg',
			title: 'Kopi Gayo',
			numRate: 4.8,
			totalRate: 90,
			location: 'Sembalun, Lombok Timur',
			price: 150000
		},
		{
			image: '/static/katalog-4.jpg',
			title: 'Kopi Papandayan',
			numRate: 4.6,
			totalRate: 72,
			location: 'Garut, Jawa Barat',
			price: 115000
		}
	];

	function formatNumber(number) {
		return number.toString().replace(/\B(?=(\d{3})+(?!\d))/g, '.');
	}
</script>

<section class="catalog">
	<div class="header mb-8 flex items-center justify-between">
		<div class="heading">
			<span class="text-xs uppercase font-semibold tracking-wider">#BijiKopi</span>
			<h3 class="w-3/4 font-mont text-3xl uppercase tracking-wider">Biji Kopi Terbaik Kami</h3>
		</div>
		<div class="cta">
			<button
				class="px-8 py-3 text-xs uppercase tracking-wider font-medium flex items-center space-x-2 border-[1.5px] border-gray-800"
			>
				<span> Lihat Semua </span>
				<div class="icon">
					<svg
						class="w-4 h-4"
						xmlns="http://www.w3.org/2000/svg"
						fill="#1f2937"
						viewBox="0 0 256 256"
						><rect width="256" height="256" fill="none" /><line
							x1="40"
							y1="128"
							x2="216"
							y2="128"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/><polyline
							points="144 56 216 128 144 200"
							fill="none"
							stroke="#1f2937"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="16"
						/></svg
					>
				</div>
			</button>
		</div>
	</div>

	<div class="list">
		<div class="wrapper grid grid-cols-4 gap-8">
			{#each catalogs as catalog}
				<div class="item">
					<!-- Image -->
					<div class="image">
						<img src={catalog.image} alt="Kopi Sajang" />
					</div>

					<!-- Title & Rate -->
					<div
						class="title-rate py-3 border-b border-b-1 border-gray-300 flex items-start justify-between"
					>
						<div class="desc">
							<h3 class="font-mont">{catalog.title}</h3>
							<span class="text-xs tracking-wide">{catalog.location}</span>
						</div>

						<div class="rate mt-1 flex items-center space-x-1 text-xs font-medium">
							<div class="icon">
								<svg
									class="w-4 h-4"
									xmlns="http://www.w3.org/2000/svg"
									fill="#1f2937"
									viewBox="0 0 256 256"
									><rect width="256" height="256" fill="none" /><path
										d="M132.4,190.7l50.4,32c6.5,4.1,14.5-2,12.6-9.5l-14.6-57.4a8.7,8.7,0,0,1,2.9-8.8l45.2-37.7c5.9-4.9,2.9-14.8-4.8-15.3l-59-3.8a8.3,8.3,0,0,1-7.3-5.4l-22-55.4a8.3,8.3,0,0,0-15.6,0l-22,55.4a8.3,8.3,0,0,1-7.3,5.4L31.9,94c-7.7.5-10.7,10.4-4.8,15.3L72.3,147a8.7,8.7,0,0,1,2.9,8.8L61.7,209c-2.3,9,7.3,16.3,15,11.4l46.9-29.7A8.2,8.2,0,0,1,132.4,190.7Z"
										fill="none"
										stroke="#1f2937"
										stroke-linecap="round"
										stroke-linejoin="round"
										stroke-width="16"
									/></svg
								>
							</div>
							<div class="number">
								<span>{catalog.numRate}</span>
							</div>
							<div class="total">
								(<span>{catalog.totalRate}</span>)
							</div>
						</div>
					</div>

					<!-- Price & CTA -->
					<div class="price-cta py-4 flex items-end justify-between">
						<div class="price flex flex-col items-start">
							<span class="text-xs">Harga</span>
							<span class="font-semibold tracking-wide">
								Rp.{formatNumber(catalog.price)},- / kg
							</span>
						</div>

						<div class="cta">
							<button
								class="uppercase bg-gray-800 hover:bg-gray-600 py-2 px-3 tracking-wider font-medium text-gray-50 text-[0.625rem]"
								>Tambah</button
							>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
