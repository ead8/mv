<script>
	const images = [
		{ src: '/images/banner.png', alt: 'Modern living room' },
		{ src: '/images/banner (1).png', alt: 'Home office' },
		{ src: '/images/banner (2).png', alt: 'Living room with fireplace' },
		{ src: '/images/image.png', alt: 'Modern bedroom' }
	];
</script>

<section class="overflow-hidden bg-[#f8f3eb] py-20">
	<div class="flex flex-col items-end pt-12">
		<div class="mx-auto max-w-[1220px] px-4">
			<div class="grid grid-cols-1 place-items-center gap-1 md:grid-cols-[1.5fr_1fr]">
		
				<!-- Main Content -->
				<div class=" text-center md:text-left">
					<h1 class="font-['Alice'] text-[36px] leading-[46px] font-normal text-center md:text-[64px] md:leading-[73.15px] md:text-left text-[#513B2B] underline-offset-auto decoration-skip-ink-none">
						Your Dream Space,
						Designed to Perfection.
					</h1>										
					<p class="mt-6 max-w-2xl text-lg text-gray-600">
						Designing bespoke interiors that inspire and captivate, blending style, functionality,
						and timeless elegance to create spaces you'll love.
					</p>
				</div>
				<!-- Full-width Carousel -->
				<div class="mt-10 block w-full md:hidden">
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
				<div class=" grid grid-cols-2 place-items-center gap-3 md:place-items-start lg:grid-cols-2 md:justify-self-end">
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

				<div class="md:justify-self-start mt-10 flex flex-col items-center gap-6 md:flex-row">
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
				<div class=" mt-10 flex justify-center gap-12 opacity-50">
					<img src="/images/logo (1).png" alt="company logo" class="w-auto grayscale md:h-12" />
				</div>
			</div>
		</div>

		<!-- Full-width Carousel -->
		<div class="mt-10 hidden w-full md:block">
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
	</div>
</section>
