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

<section class="bg-[#F5EFE6] py-20">
	<div class="flex flex-col md:items-end max-w-[1440px] px-4">
		<!-- Section Header -->
		<div class="mx-auto mb-16 text-center">
			<h2 class="mb-6 font-serif text-4xl text-[#5C4937] lg:text-5xl">Awards & Recognitions</h2>
			<p class=" leading-relaxed text-[#766D66]">
				Celebrating our journey of excellence and creativity with prestigious accolades that reflect
				our dedication and success.
			</p>
		</div>

		<!-- Awards Grid -->
		<div class="flex overflow-x-auto gap-8 pb-4 snap-x snap-mandatory max-w-[1220px]">
			{#each awards as award}
				<div class="group min-w-[300px] snap-center">
					<!-- Certificate Image -->
					<div class="mb-4 rounded-2xl bg-white p-4 shadow-sm transition-all duration-300 hover:shadow-md">
						<img 
							src={award.image} 
							alt={award.title} 
							class="rounded-lg h-[350px] w-[300px] md:h-[457px] md:w-full object-cover" 
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
</section>
