<script lang="ts">
  // Logos would typically be imports, using text placeholders or SVGs for now
  const logos = [
    "Allianz",
    "BMW",
    "Lufthansa",
    "Spotify",
    "Red Bull"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#2a1b5e] via-[#d4a8a8] to-[#fdfbf7] text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#2e2166_0%,#8c5e8f_40%,#e6b99c_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Your 0 to 1 Partner for Digital Innovation. <span class="text-gray-500">Blending consultancy expertise with agency craft and creativity, we lead ambitious companies from Insight to Impact—fast.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
