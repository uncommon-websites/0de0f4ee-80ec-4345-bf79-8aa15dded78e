<script lang="ts">
  const stats = [
    {
      label: "37+ Years",
      desc: "Since 1987, we've been serving our community with integrity and expertise. Three generations of the founding family have grown this dealership from a small lot to a trusted automotive destination. Our longevity speaks to our commitment to doing business the right way.",
      img: "/generated/image-happy-family-of-three-generations-standi-1765523539778-1.webp"
    },
    {
      label: "15,000+ Vehicles Sold",
      desc: "Over fifteen thousand families have trusted us with their vehicle needs. Each sale represents a relationship built on transparency, fair pricing, and genuine care. Our customers return generation after generation because we deliver on our promises.",
      img: "/generated/image-satisfied-customers-receiving-keys-to-th-1765523543898-3.webp"
    },
    {
      label: "98% Satisfaction",
      desc: "Our customer satisfaction rating isn't just a number—it's a reflection of our dedication to service excellence. From your first visit to years of maintenance, we're committed to exceeding expectations at every touchpoint. Your satisfaction is our success.",
      img: "/generated/image-professional-car-salesperson-consulting--1765523541880-2.webp"
    },
    {
      label: "3 Generations",
      desc: "Grandfather, father, and son—three generations working together under one roof. This multi-generational expertise means we combine time-tested wisdom with modern innovation. When you work with us, you get the benefit of decades of automotive knowledge.",
      img: "/generated/image-happy-family-of-three-generations-standi-1765523539778-1.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Numbers tell a story. Here's a snapshot of our legacy, our commitment, and the trust our community has placed in us over the decades.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
