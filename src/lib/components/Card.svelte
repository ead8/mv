<script lang="ts">
  export let title: string = "";
  export let description: string = "";
  export let image: string = "";
  export let features: string[] = [];
  export let reverse: boolean = false; 
</script>

<div class="flex flex-col lg:flex-row items-center gap-8 p-6" class:lg:flex-row-reverse={reverse}>
  <img 
    src={image} 
    alt={title} 
    class="w-full lg:w-1/2 rounded-lg object-cover"
  />
  <div class="flex-1">
    <h2 class="text-4xl text-[#594431] font-alice mb-4">{title}</h2>
    <p class="text-gray-600 font-raleway mb-6">{description}</p>
    <div class="space-y-3">
      {#each features as feature}
        <div class="flex items-center gap-2">
          <svg viewBox="0 0 24 24" class="w-5 h-5 text-gray-600" fill="currentColor">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/>
          </svg>
          <span>{feature}</span>
        </div>
      {/each}
    </div>
  </div>
</div>
