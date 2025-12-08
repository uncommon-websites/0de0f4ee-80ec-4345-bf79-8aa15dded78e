<script lang="ts">
  const photos = [
    {
      title: "Fitness Meets Work",
      desc: "Stay healthy with our dedicated gym and personal training part of our employee wellness program.",
      img: "https://images.unsplash.com/photo-1534438327276-14e5300c3a48?auto=format&fit=crop&q=80&w=400"
    },
    {
      title: "Your Social Hub",
      desc: "Located in vibrant city centers, our offices are places for connection and face-to-face collaboration.",
      img: "https://images.unsplash.com/photo-1527192491265-7e15c55b1ed2?auto=format&fit=crop&q=80&w=400"
    },
    {
      title: "Fueling Creativity",
      desc: "We care about good food—our in-house chef ensures everyone stays energized and inspired.",
      img: "https://images.unsplash.com/photo-1511632765486-a01980e01a18?auto=format&fit=crop&q=80&w=400"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on people, not just projects.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      In a world of digital meetings, we value face-to-face connections. Our culture is built on trust, freedom, and support, fostering personal growth and collaboration that goes beyond just completing tasks—it's about enjoying the journey together.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
