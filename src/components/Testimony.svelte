<script>
	let testimonies = [
		{
			profileImage: '/static/testimony-2.jpg',
			profileName: 'Afochar Syabnirusmanto',
			profileOccupation: 'Kang Ngopi',
			description: 'Saya telah mencoba berbagai jenis kopi dari bermacam sumber. Dan Inokulen TOP!',
			numRate: 4.5
		},
		{
			profileImage: './static/testimony-1.jpg',
			profileName: 'Kateline Ellice',
			profileOccupation: 'Coffee Lovers',
			description:
				'Biji kopi dari Inokulen merupakan biji kopi terbaik pilihan, dengan keunikannya tersendiri',
			numRate: 4.5
		}
	];
</script>

<section class="testimonies text-sm px-24 py-16 bg-gray-100">
	<div class="wrapper grid grid-cols-12 gap-x-16">
		<div class="testimony col-span-8 grid grid-cols-2 gap-x-8">
			{#each testimonies as testimony}
				<div
					class="card p-8 border-[1.5px] border-dashed border-gray-800 flex flex-col items-center space-y-4"
				>
					<!-- Image -->
					<div class="image">
						<img
							class="w-12 h-12 rounded-full object-cover"
							src={testimony.profileImage}
							alt="Testimony"
						/>
					</div>

					<!-- Description -->
					<div class="description">
						<p class="text-center">
							{testimony.description}
						</p>
					</div>

					<!-- Star -->
					<div class="stars flex items-center space-x-2">
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.366 1.95134C7.566 1.33734 8.43467 1.33734 8.634 1.95134L9.64667 5.06734C9.69025 5.201 9.77497 5.31746 9.88872 5.40008C10.0025 5.4827 10.1394 5.52724 10.28 5.52734H13.5567C14.2027 5.52734 14.4707 6.35401 13.9487 6.73401L11.298 8.65934C11.1841 8.74212 11.0994 8.85881 11.0559 8.9927C11.0125 9.12659 11.0125 9.2708 11.056 9.40468L12.068 12.5207C12.268 13.1353 11.5647 13.646 11.0427 13.266L8.392 11.3407C8.27808 11.2579 8.14085 11.2133 8 11.2133C7.85916 11.2133 7.72193 11.2579 7.608 11.3407L4.95734 13.266C4.43534 13.646 3.732 13.1347 3.932 12.5207L4.944 9.40468C4.98752 9.2708 4.98755 9.12659 4.94407 8.9927C4.9006 8.85881 4.81586 8.74212 4.702 8.65934L2.05134 6.73401C1.52867 6.35401 1.798 5.52734 2.44334 5.52734H5.71934C5.86003 5.52738 5.99714 5.4829 6.11102 5.40028C6.2249 5.31765 6.30972 5.20111 6.35334 5.06734L7.366 1.95134V1.95134Z"
								stroke="#FBBF24"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.366 1.95134C7.566 1.33734 8.43467 1.33734 8.634 1.95134L9.64667 5.06734C9.69025 5.201 9.77497 5.31746 9.88872 5.40008C10.0025 5.4827 10.1394 5.52724 10.28 5.52734H13.5567C14.2027 5.52734 14.4707 6.35401 13.9487 6.73401L11.298 8.65934C11.1841 8.74212 11.0994 8.85881 11.0559 8.9927C11.0125 9.12659 11.0125 9.2708 11.056 9.40468L12.068 12.5207C12.268 13.1353 11.5647 13.646 11.0427 13.266L8.392 11.3407C8.27808 11.2579 8.14085 11.2133 8 11.2133C7.85916 11.2133 7.72193 11.2579 7.608 11.3407L4.95734 13.266C4.43534 13.646 3.732 13.1347 3.932 12.5207L4.944 9.40468C4.98752 9.2708 4.98755 9.12659 4.94407 8.9927C4.9006 8.85881 4.81586 8.74212 4.702 8.65934L2.05134 6.73401C1.52867 6.35401 1.798 5.52734 2.44334 5.52734H5.71934C5.86003 5.52738 5.99714 5.4829 6.11102 5.40028C6.2249 5.31765 6.30972 5.20111 6.35334 5.06734L7.366 1.95134V1.95134Z"
								stroke="#FBBF24"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.366 1.95134C7.566 1.33734 8.43467 1.33734 8.634 1.95134L9.64667 5.06734C9.69025 5.201 9.77497 5.31746 9.88872 5.40008C10.0025 5.4827 10.1394 5.52724 10.28 5.52734H13.5567C14.2027 5.52734 14.4707 6.35401 13.9487 6.73401L11.298 8.65934C11.1841 8.74212 11.0994 8.85881 11.0559 8.9927C11.0125 9.12659 11.0125 9.2708 11.056 9.40468L12.068 12.5207C12.268 13.1353 11.5647 13.646 11.0427 13.266L8.392 11.3407C8.27808 11.2579 8.14085 11.2133 8 11.2133C7.85916 11.2133 7.72193 11.2579 7.608 11.3407L4.95734 13.266C4.43534 13.646 3.732 13.1347 3.932 12.5207L4.944 9.40468C4.98752 9.2708 4.98755 9.12659 4.94407 8.9927C4.9006 8.85881 4.81586 8.74212 4.702 8.65934L2.05134 6.73401C1.52867 6.35401 1.798 5.52734 2.44334 5.52734H5.71934C5.86003 5.52738 5.99714 5.4829 6.11102 5.40028C6.2249 5.31765 6.30972 5.20111 6.35334 5.06734L7.366 1.95134V1.95134Z"
								stroke="#FBBF24"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.366 1.95134C7.566 1.33734 8.43467 1.33734 8.634 1.95134L9.64667 5.06734C9.69025 5.201 9.77497 5.31746 9.88872 5.40008C10.0025 5.4827 10.1394 5.52724 10.28 5.52734H13.5567C14.2027 5.52734 14.4707 6.35401 13.9487 6.73401L11.298 8.65934C11.1841 8.74212 11.0994 8.85881 11.0559 8.9927C11.0125 9.12659 11.0125 9.2708 11.056 9.40468L12.068 12.5207C12.268 13.1353 11.5647 13.646 11.0427 13.266L8.392 11.3407C8.27808 11.2579 8.14085 11.2133 8 11.2133C7.85916 11.2133 7.72193 11.2579 7.608 11.3407L4.95734 13.266C4.43534 13.646 3.732 13.1347 3.932 12.5207L4.944 9.40468C4.98752 9.2708 4.98755 9.12659 4.94407 8.9927C4.9006 8.85881 4.81586 8.74212 4.702 8.65934L2.05134 6.73401C1.52867 6.35401 1.798 5.52734 2.44334 5.52734H5.71934C5.86003 5.52738 5.99714 5.4829 6.11102 5.40028C6.2249 5.31765 6.30972 5.20111 6.35334 5.06734L7.366 1.95134V1.95134Z"
								stroke="#FBBF24"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
						<svg
							width="16"
							height="16"
							viewBox="0 0 16 16"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M7.366 1.95134C7.566 1.33734 8.43467 1.33734 8.634 1.95134L9.64667 5.06734C9.69025 5.201 9.77497 5.31746 9.88872 5.40008C10.0025 5.4827 10.1394 5.52724 10.28 5.52734H13.5567C14.2027 5.52734 14.4707 6.35401 13.9487 6.73401L11.298 8.65934C11.1841 8.74212 11.0994 8.85881 11.0559 8.9927C11.0125 9.12659 11.0125 9.2708 11.056 9.40468L12.068 12.5207C12.268 13.1353 11.5647 13.646 11.0427 13.266L8.392 11.3407C8.27808 11.2579 8.14085 11.2133 8 11.2133C7.85916 11.2133 7.72193 11.2579 7.608 11.3407L4.95734 13.266C4.43534 13.646 3.732 13.1347 3.932 12.5207L4.944 9.40468C4.98752 9.2708 4.98755 9.12659 4.94407 8.9927C4.9006 8.85881 4.81586 8.74212 4.702 8.65934L2.05134 6.73401C1.52867 6.35401 1.798 5.52734 2.44334 5.52734H5.71934C5.86003 5.52738 5.99714 5.4829 6.11102 5.40028C6.2249 5.31765 6.30972 5.20111 6.35334 5.06734L7.366 1.95134V1.95134Z"
								stroke="#FBBF24"
								stroke-linecap="round"
								stroke-linejoin="round"
							/>
						</svg>
					</div>

					<!-- Profile -->
					<div class="profile flex items-center flex-col">
						<h4 class="mb-2 font-mont text-center">{testimony.profileName}</h4>
						<span class="text-sm text-gray-500">{testimony.profileOccupation}</span>
					</div>
				</div>
			{/each}
		</div>

		<!-- Header -->
		<div class="header h-full col-span-4 mb-8 flex flex-col items-start justify-between">
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
	</div>
</section>
