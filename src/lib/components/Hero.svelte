<script lang="ts">
  // Automotive brand partnerships
  const brands = [
    "Ford",
    "Chevrolet",
    "Toyota",
    "Honda",
    "Nissan"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-black text-white">
  <!-- Background image overlay -->
  <div class="absolute inset-0 z-0">
    <img src="/generated/image-modern-car-dealership-showroom-interior--1765523537386-0.webp" alt="Dealership Showroom" class="w-full h-full object-cover opacity-40" />
    <div class="absolute inset-0 bg-gradient-to-t from-black via-black/60 to-transparent"></div>
  </div>

  <div class="max-w-4xl mb-32 pt-40 relative z-10">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Trusted Vehicle Ownership Through Multi-Generational Expertise. <span class="text-gray-400">Family-owned since 1987, we deliver personalized service and automotive excellence that spans generations.</span>
    </h1>
  </div>

  <div class="border-t border-gray-700 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 relative z-10">
    {#each brands as brand}
      <div class="h-8 flex items-center justify-center font-bold text-xl">{brand}</div>
    {/each}
    <!-- Additional brand placeholders -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
