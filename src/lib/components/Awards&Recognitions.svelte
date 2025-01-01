<script>
	const awards = [
		{
			image: '/images/Picture8.png', // Replace with your actual certificate image
			title: 'Inaugural Women of Excellence Awards',
			year: '2014'
		},
		{
			image: '/images/Picture42.png', // Replace with your actual certificate image
			title: 'MALAYSIA MEGA SALE CARNIVAL',
			year: '2009'
		},
		{
			image: '/images/Picture42.png', // Replace with your actual certificate image
			title: 'Nippon Paint Young Designer',
			year: '2013'
		}
	];
</script>

<section class="bg-[#F5EFE6] py-10">
	<div class="mx-auto flex max-w-[1220px] flex-col px-4 md:items-end">
		<!-- Section Header -->
		<div class="mx-auto mb-16 text-center">
			<h2 class="mb-6 font-serif text-4xl text-[#5C4937] lg:text-5xl">Awards & Recognitions</h2>
			<p class=" font-raleway text-lg leading-relaxed text-[#766D66]">
				Celebrating our journey of excellence and creativity with prestigious accolades that reflect
				our dedication and success.
			</p>
		</div>

		<!-- Awards Grid -->
		<div class="relative w-full">
			<div class="flex snap-x snap-mandatory gap-[14px] overflow-x-auto pb-4">
				{#each awards as award}
					<div class="group min-w-[300px] flex-shrink-0 snap-center">
						<!-- Certificate Image -->
						<div
							class="mb-4 rounded-2xl bg-white p-4 shadow-sm transition-all duration-300 hover:shadow-md"
						>
							<img
								src={award.image}
								alt={award.title}
								class="h-[350px] w-[300px] rounded-lg object-cover md:h-[457px] md:w-full"
							/>
						</div>

						<!-- Award Info -->
						<div>
							<h3 class="font-serif text-xl text-[#5C4937]">
								{award.title}
							</h3>
							<p class="text-gray-600">
								{award.year}
							</p>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>
