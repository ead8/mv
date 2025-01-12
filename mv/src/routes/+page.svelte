<script>
	import Aboutus from '../lib/components/Aboutus.svelte';
	import AwardsRecognitions from '../lib/components/Awards&Recognitions.svelte';
	import Contactus from '../lib/components/Contactus.svelte';
	import Hero from '../lib/components/Hero.svelte';
	import LastProjects from '../lib/components/LastProjects.svelte';
	import Testimonial from '../lib/components/Testimonial.svelte';
	import Vedios from '../lib/components/Vedios.svelte';
	import Work from '../lib/components/Work.svelte';
	import { LightbulbIcon, Building2Icon, GraduationCapIcon, Award, Play } from 'lucide-svelte';

	const features = [
		{
			icon: LightbulbIcon,
			title: 'Creative Skill Development',
			description: 'Industry-focused training under HRDF, enhancing workforce expertise.'
		},
		{
			icon: Award,
			title: 'Recognized Provider',
			description: 'Certified by HRD Corp, offering expert arts and interior design training.'
		},
		{
			icon: Building2Icon,
			title: 'Real Estate Training',
			description: 'High-end real estate and programs through Advisors Group.'
		},
		{
			icon: GraduationCapIcon,
			title: 'Expert Trainers',
			description: 'Workshops by certified trainers in traditional, contemporary, and digital art.'
		}
	];
	const steps = [
		{
			number: '01',
			title: 'Understanding Your Vision',
			description:
				'With over 20 years of expertise, we work closely with clients to understand their unique needs and aspirations, ensuring every design is tailored to their vision.',
			images: ['/images/Rectangle 14.png', '/images/Frame 108.png']
		},
		{
			number: '02',
			title: 'Collaborating to Create',
			description:
				'Partner with our expert designers to craft bespoke solutions. From functional layouts to artistic details, we bring your ideas to life with precision and creativity.',
			images: ['/images/Rectangle 15.png', '/images/Rectangle 14 (1).png']
		},
		{
			number: '03',
			title: 'Seamless Execution',
			description:
				'We source premium materials and trusted partners to ensure every design is executed flawlessly, transforming concepts into functional spaces.',
			images: ['/images/Rectangle 14.png', '/images/Frame 108.png']
		}
	];

</script>

<Hero />

<Aboutus />

<section class="bg-[#EBE2D5] py-16">
	<div class=" mx-auto px-4 md:w-[1091px]">
		<!-- Heading -->
		<div class="text-center ">
			<h2 class="text-3xl font-bold text-[#5A4635] md:text-4xl">Our Services</h2>
			<p class="mx-auto mt-4 text-lg text-[#766D66]">
				Discover a wide range of professional design solutions crafted to transform your vision into
				reality. From planning and architecture to bespoke interiors and training programs, we bring
				creativity and expertise to every project.
			</p>
		</div>

		<!-- Services Grid -->
		<div class="mt-12 grid grid-cols-1 gap-4 sm:grid-cols-2 lg:grid-cols-3">
			<!-- Service 1 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3]">
				<div class="flex justify-center">
					<img src="/icons/Frame.svg" alt="Planning Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Planning</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					We create strategic, detailed plans for seamless execution and optimal results.
				</p>
			</div>

			<!-- Service 2 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (1).svg" alt="Architecture Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Architecture</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					We create sustainable, functional, and aesthetically inspiring architectural designs.
				</p>
			</div>

			<!-- Service 3 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (2).svg" alt="Interior Design Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Interior Design</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					Transform your spaces into beautiful, functional, and personalized environments.
				</p>
			</div>

			<!-- Service 4 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (3).svg" alt="Landscape Design Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Landscape Design</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					We design outdoor spaces that blend nature and structure, creating serene environments.
				</p>
			</div>

			<!-- Service 5 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (4).svg" alt="Lighting Design Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Lighting Design</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					Enhance your spaces with lighting that adds ambiance, functionality, and elegance.
				</p>
			</div>

			<!-- Service 6 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (5).svg" alt="Graphics Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Graphics</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					Bring your ideas to life with graphic designs that captivate and communicate effectively.
				</p>
			</div>

			<!-- Service 7 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl hover:bg-[#E9E0D3] ">
				<div class="flex justify-center">
					<img src="/icons/Frame (6).svg" alt="Paintings Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Paintings/Art Pieces</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					Add character to your spaces with custom or curated art pieces that resonate with your
					style.
				</p>
			</div>

			<!-- Service 8 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl ">
				<div class="flex justify-center">
					<img src="/icons/Frame (7).svg" alt="Art Gallery Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Art Gallery</h3>
				<p class="mt-1 font-raleway text-sm text-[#6A6866]">
					Explore our virtual gallery featuring exceptional works by talented artists and graduates.
				</p>
			</div>

			<!-- Service 9 -->
			<div class="text-center rounded-[12px] p-3 hover:shadow-xl ">
				<div class="flex justify-center">
					<img src="/icons/Frame (8).svg" alt="Workshop Icon" class="mb-4 h-12 w-12" />
				</div>
				<h3 class="text-lg font-semibold text-[#5A4635] font-alice">Workshop & Training Provider</h3>
				<p class="mt-1 font-raleway text-sm text-gray-600">
					Empowering individuals with skills in arts, design, and real estate through certified
					training.
				</p>
			</div>
		</div>
	</div>
</section>

<section class="bg-white px-4 py-16">
	<div class="mx-auto md:max-w-6xl">
		<h2 class="mb-20 text-center font-serif text-5xl text-[#5C4937]">How We Work</h2>

		<div class="relative w-full">
			<div class="flex overflow-x-auto snap-x snap-mandatory gap-8 pb-4 max-w-[95%]">
				{#each steps as step}
					<div class="snap-start flex-none w-[300px] md:w-[400px] flex-shrink-0 flex flex-col space-y-6">
						<!-- Number -->
						<div
							class="flex h-8 w-8 items-center justify-center rounded-full bg-[#5C4937] text-sm font-medium text-white md:h-12 md:w-12 md:text-lg"
						>
							{step.number}
						</div>

						<!-- Content -->
						<div class="space-y-4">
							<h3 class="font-alice text-2xl text-[#5A4635]">{step.title}</h3>
							<p class="leading-relaxed font-raleway text-[#6A6866]">
								{step.description}
							</p>
						</div>

						<!-- Image Grid -->
						<div class="mt-6 grid grid-cols-2 gap-2">
							{#each step.images as image}
								<img
									src={image}
									alt="Interior design"
									class="h-48 w-full rounded-lg object-cover"
									loading="lazy"
								/>
							{/each}
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>

<section class="bg-[#E9E0D3] py-20">
	<div class="mx-auto max-w-7xl px-4">
		<div class="grid gap-16 lg:grid-cols-2">
			<!-- Left Column - Hero Text -->
			<div class="space-y-6">
				<h1 class="font-alice text-3xl leading-tight text-[#5A4635] md:text-5xl">
					Empowering Creativity,<br />
					Shaping the Future with<br />
					MZ Design Consultancy
				</h1>

				<p class="max-w-xl font-raleway md:text-lg leading-relaxed text-[#766D66]">
					Transform your skills and unleash your creative potential with MZ Design Consultancy. We
					offer world-class training in arts, interior design, and real estate, empowering
					individuals and professionals to excel and innovate in their fields.
				</p>
			</div>

			<!-- Right Column - Features Grid -->
			<div class="grid gap-6 md:grid-cols-2">
				{#each features as feature}
					<div
						class="space-y-4 font-raleway rounded-lg border-[1.5px] border-[#766D660F] bg-[#E9E0D3] p-6 shadow-[0px_8px_64px_0px_#5A46351A]"
					>
						<svelte:component
							this={feature.icon}
							class="h-6 w-6 text-[#5C4937] shadow-[0px_8px_64px_0px_#8F8F8F29]"
						/>
						<h3 class="font-serif text-lg text-[#5C4937]">
							{feature.title}
						</h3>
						<p class="text-[#766D66]">
							{feature.description}
						</p>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>

<Work/>

<LastProjects/>

<AwardsRecognitions/>

<Vedios/>

<Testimonial/>

<Contactus />
