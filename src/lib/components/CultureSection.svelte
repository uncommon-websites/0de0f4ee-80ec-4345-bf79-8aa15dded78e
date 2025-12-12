<script lang="ts">
  const cards = [
    {
      title: "We're Not Just a Dealership...",
      subtitle: "We're Your Automotive Family.",
      image: "/generated/image-happy-family-of-three-generations-standi-1765523539778-1.webp"
    },
    {
      title: "We Don't Just Sell Cars...",
      subtitle: "We Build Lasting Relationships.",
      image: "/generated/image-professional-car-salesperson-consulting--1765523541880-2.webp"
    },
    {
      title: "We Don't Just Make Sales...",
      subtitle: "We Create Happy Customers.",
      image: "/generated/image-satisfied-customers-receiving-keys-to-th-1765523543898-3.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Family values aren't just words to us—they're our foundation. Three generations of automotive expertise mean we treat every customer like family, building relationships that last a lifetime.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
