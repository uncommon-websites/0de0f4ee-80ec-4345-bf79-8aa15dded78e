<script lang="ts">
  const projects = [
    {
      client: "Red Bull",
      desc: "A global platform built to Scale, Evolve, and Perform.",
      bg: "bg-[#000c2d]",
      img: "", // Placeholder logic handled in template
      dark: true
    },
    {
      client: "Volvo",
      desc: "Redefining how people experience insurance.",
      bg: "bg-gray-200",
      img: "https://images.unsplash.com/photo-1556742049-0cfed4f7a07d?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "The Organics",
      desc: "Translating a refreshing identity into a bold platform.",
      bg: "bg-[#8da356]",
      img: "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "Isar Aerospace",
      desc: "Launching a brand journey into orbit.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      client: "REWE",
      desc: "Digital Convenience in your Pocket.",
      bg: "bg-[#f0f0f0]",
      img: "https://images.unsplash.com/photo-1512428559087-560fa5ce7d87?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true // Making REWE full width to align last two items
    },
    {
      client: "Alpha Tauri",
      desc: "Designing the interface of wearable intelligence.",
      bg: "bg-[#e0e0e0]",
      img: "https://images.unsplash.com/photo-1551650975-87deedd944c3?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "Zalando",
      desc: "Designing the Zalando E-Commerce Operating System.",
      bg: "bg-[#d8c5f0]",
      img: "https://images.unsplash.com/photo-1555421689-49263376da7a?auto=format&fit=crop&q=80&w=800",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We orchestrate strategy, design, and technology</span> to create digital experiences that connect with millions and give you the edge that sets you apart.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
