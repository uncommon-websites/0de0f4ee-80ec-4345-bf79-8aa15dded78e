<script lang="ts">
  const offerings = [
    {
      client: "New Vehicles",
      desc: "Latest models from trusted manufacturers with competitive pricing and financing.",
      bg: "bg-black",
      img: "/generated/image-sleek-new-luxury-sedan-in-modern-showroo-1765523556602-9.webp",
      dark: true
    },
    {
      client: "Pre-Owned Vehicles",
      desc: "Quality certified pre-owned vehicles inspected by our expert technicians.",
      bg: "bg-gray-200",
      img: "/generated/image-row-of-quality-pre-owned-vehicles-on-dea-1765523554451-8.webp",
      dark: false
    },
    {
      client: "Financing Solutions",
      desc: "Flexible financing options tailored to your budget and lifestyle.",
      bg: "bg-[oklch(0.696_0.17_162.48)]",
      img: "",
      dark: false
    },
    {
      client: "Service & Maintenance",
      desc: "Expert automotive service from certified technicians who care.",
      bg: "bg-gray-900",
      img: "/generated/image-clean-modern-car-service-center-with-tec-1765523546108-4.webp",
      dark: true
    },
    {
      client: "Trade-In Program",
      desc: "Get the best value for your current vehicle with our fair trade-in process.",
      bg: "bg-[#f0f0f0]",
      img: "",
      dark: false,
      full: true
    },
    {
      client: "Parts & Accessories",
      desc: "Genuine OEM parts and quality accessories for your vehicle.",
      bg: "bg-[#e0e0e0]",
      img: "",
      dark: false
    },
    {
      client: "Extended Warranties",
      desc: "Protect your investment with comprehensive warranty coverage.",
      bg: "bg-gray-100",
      img: "",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We combine family values with modern service</span> to deliver a vehicle ownership experience that's personal, trustworthy, and built to last generations.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each offerings as offering}
      <div class="group cursor-pointer {offering.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${offering.bg} mb-4 ${offering.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if offering.img}
             <img src={offering.img} alt={offering.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for service icons on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${offering.dark ? 'text-white' : 'text-black'}`}>{offering.client}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{offering.client}</h3>
        <p class="text-sm text-gray-600">{offering.desc}</p>
      </div>
    {/each}
  </div>
</section>
