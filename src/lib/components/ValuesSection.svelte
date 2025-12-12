<script lang="ts">
  const photos = [
    {
      title: "State-of-the-Art Service",
      desc: "Our modern service center features the latest diagnostic equipment and certified technicians dedicated to your vehicle's care.",
      img: "/generated/image-clean-modern-car-service-center-with-tec-1765523546108-4.webp"
    },
    {
      title: "Comfortable Experience",
      desc: "Relax in our customer lounge with complimentary refreshments, WiFi, and comfortable seating while we service your vehicle.",
      img: "/generated/image-comfortable-customer-waiting-area-in-car-1765523548269-5.webp"
    },
    {
      title: "Expert Technicians",
      desc: "Our ASE-certified technicians bring decades of combined experience and treat every vehicle with meticulous attention to detail.",
      img: "/generated/image-professional-automotive-technician-inspe-1765523550306-6.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on experience, not just transactions.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      From our modern showroom to our service center, every detail is designed with you in mind. We've created a welcoming environment where you can make informed decisions, relax during service visits, and trust that your vehicle is in expert hands.
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
