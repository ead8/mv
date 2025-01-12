<script>
  export let title = "";
  export let subtitle = "";
  export let image = "";
</script>

<a href="/portfolio-details" class="block">
  <div class="rounded-lg overflow-hidden">
      <!-- Image Section -->
      <div class="overflow-hidden">
          <img 
              src={image} 
              alt={title} 
              class="w-full object-cover transform transition-transform duration-300 hover:scale-[1.03]" 
          />
      </div>

      <!-- Content Section -->
      <div class="p-4 text-center">
          <h3 class="text-lg font-semibold font-raleway text-[#6b4c35]">{title}</h3>
          <p class="text-gray-600 text-sm font-raleway">{subtitle}</p>
      </div>
  </div>
</a>
