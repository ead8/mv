<script>
    	const contacts = [
		{
			id: 1,
			icon: '/icons/email.png', // Replace with an icon component or SVG
			title: 'Email',
			detail: 'support@gulaly.com',
			buttonLabel: 'CONTACT'
		},
		{
			id: 2,
			icon: '/icons/phone.png', // Replace with an icon component or SVG
			title: 'Phone',
			detail: 'Office. +61 234–567 8910',
			buttonLabel: 'CALL'
		},
		{
			id: 3,
			icon: '/icons/place.png', // Replace with an icon component or SVG
			title: 'Office',
			detail: '6391 Elgin St. Celina, Delaware 10299',
			buttonLabel: 'LOCATION'
		}
	];
</script>

<section class="bg-[#F5EFE6] pt-12">
	<div class="mx-auto max-w-[1260px] px-4 text-center">
        <div class="flex flex-col items-center justify-center">
            <h2 class="mb-4 text-[50px] font-normal font-alice leading-[57.15px] text-center text-[#6b4c35] underline-offset-[from-font] decoration-skip-ink-none">Contact Us</h2>
            <p class="mb-10 max-w-[700px] font-raleway text-lg text-[#766D66]">
                Get in touch with us for your design needs. Whether it’s a question, a project inquiry, or
                feedback, we’re here to help.
            </p>
        </div>
		<div class="grid grid-cols-1 gap-6 md:grid-cols-3">
			{#each contacts as contact}
				<div class="rounded-xl border border-[#766D66] bg-[#F5EFE6] p-6 text-left shadow-md">
					<div class="mb-4 ">
						<img class="flex-shrink-0 text-2xl text-[#6b4c35]" 
							src={contact.icon}
                            alt={contact.title}
						/>
						<h3 class="text-lg mt-2 font-semibold m text-[#6b4c35]">{contact.title}</h3>
					</div>
					<p class="mb-4 font-general-sans text-sm font-semibold leading-6 text-left text-[#5A4635] underline-offset-[from-font] decoration-skip-ink-none">
						{#if contact.title === 'Phone'}
							<span>Office. </span><span class="underline">+61 234–567 8910</span>
						{:else}
							{contact.detail}
						{/if}
					</p>									 
					<div class="flex gap-2">
                        <button
						class="rounded-full bg-[#6b4c35] px-4 py-2 text-sm text-white transition hover:bg-opacity-80"
					>
						{contact.buttonLabel}
					</button>
					<p class="mt-2 text-xs text-gray-500">*extra information(optional)</p>
                    </div>
				</div>
			{/each}
		</div>
	</div>
</section>