<script>
	import PortfolioCard from "$lib/components/PortfolioCard.svelte";

  
    const portfolioItems = [
      {
        title: "Airlie Gardens",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio.png",
      },
      {
        title: "Gulf Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio2.png",
      },
      {
        title: "Muscat Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio3.png",
      },
      {
        title: "Gulf Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio2.png",
      },
      {
        title: "Muscat Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio3.png",
      },
      {
        title: "Airlie Gardens",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio.png",
      },
      {
        title: "Gulf Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio2.png",
      },
      {
        title: "Airlie Gardens",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio.png",
      },
      {
        title: "Muscat Villa",
        subtitle: "Middle East",
        image: "/images/portfolio/portfolio3.png",
      },
    ];
  </script>
  
  <section class="bg-[#f8f4e7] py-12">
    <div class="max-w-7xl mx-auto px-4 text-center">
      <h2 class="text-3xl font-bold font-alice text-[#6b4c35] mb-8">Portfolio</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
        {#each portfolioItems as item}
          <PortfolioCard
            title={item.title}
            subtitle={item.subtitle}
            image={item.image}
          />
        {/each}
      </div>
    </div>
  </section>
  