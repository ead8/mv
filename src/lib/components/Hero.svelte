<script>
	const images = [
		{ src: '/images/banner.png', alt: 'Modern living room' },
		{ src: '/images/banner (1).png', alt: 'Home office' },
		{ src: '/images/banner (2).png', alt: 'Living room with fireplace' },
		{ src: '/images/image.png', alt: 'Modern bedroom' }
	];
</script>

<section class="overflow-hidden bg-[#f8f3eb] py-20">
	<div class="mx-auto max-w-7xl px-6 pt-10">
		<div class="grid grid-cols-1 place-items-center gap-1 md:grid-cols-2">
			<!-- Main Content -->
			<div class="order-1 mx-2 text-center md:mx-0 md:text-left">
				<h1 class="font-serif text-3xl leading-tight text-[#513B2B] md:text-6xl">
					Your Dream Space,<br />
					Designed to Perfection.
				</h1>
				<p class="mt-6 max-w-2xl text-lg text-gray-600">
					Designing bespoke interiors that inspire and captivate, blending style, functionality, and
					timeless elegance to create spaces you'll love.
				</p>
			</div>

			<!-- Carousel Images -->
			<div class="order-2 col-span-full mt-10 w-full overflow-hidden md:order-4 md:col-span-2">
				<div class="flex animate-scroll gap-4">
					{#each [...images, ...images] as { src, alt }, i (i)}
						<div class="w-full flex-none px-2 md:w-1/2 lg:w-1/3">
							<div class="overflow-hidden rounded-xl shadow-lg">
								<img {src} {alt} class="h-48 w-full rounded-lg object-cover md:h-64" />
							</div>
						</div>
					{/each}
				</div>
			</div>

			<!-- Awards Grid -->
			<div class="order-3 mx-auto md:order-2 md:mx-0 md:justify-self-end">
				<div class="grid grid-cols-2 place-items-center gap-3 md:place-items-start lg:grid-cols-2">
					<div class="h-28 w-48 rounded-lg p-6">
						<div class="mb-3 flex items-center justify-center">
							<img src="/star.svg" alt="" class="h-8" />
						</div>
						<p class="text-center text-sm text-gray-600">
							Inaugural Women of Excellence Awards (2014)
						</p>
					</div>
					<div class="h-28 w-48 rounded-lg p-6">
						<div class="mb-3 flex items-center justify-center">
							<img src="/star2.svg" alt="" class="h-8" />
						</div>
						<p class="text-center text-sm text-gray-600">
							Awarded the Nippon Paint Young Designer Award (2013)
						</p>
					</div>
					<div class="h-28 w-48 rounded-lg p-6">
						<div class="mb-3 flex items-center justify-center">
							<img src="/star.svg" alt="" class="h-8" />
						</div>
						<p class="text-center text-sm text-gray-600">
							Nippon Paint Young Designer Award (2013)
						</p>
					</div>
					<div class="h-28 w-48 rounded-lg p-6">
						<div class="mb-3 flex items-center justify-center">
							<img src="/star2.svg" alt="" class="h-8" />
						</div>
						<p class="text-center text-sm text-gray-600">Malaysia Mega Sale Carnival (2009)</p>
					</div>
				</div>
			</div>

			<div class="order-4 mt-10 flex flex-col items-center gap-6 md:order-3 md:flex-row">
				<button
					class="rounded-full border border-[#513B2B] px-6 py-2 font-medium text-[#513B2B] transition-colors hover:bg-[#513B2B] hover:text-white"
				>
					View Our Portfolio
				</button>
				<p class="text-gray-600">
					Over <span class="font-semibold text-blue-600">100+</span> premium designs
				</p>
			</div>
			<!-- Company Logos -->
			<div class="order-4 mt-10 flex justify-center gap-12 opacity-50 md:order-3">
				<img src="/images/logo (1).png" alt="company logo" class="h-12 w-auto grayscale" />
			</div>
		</div>
	</div>
</section>
