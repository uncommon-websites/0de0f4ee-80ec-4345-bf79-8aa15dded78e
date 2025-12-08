<script lang="ts">
  const stats = [
    {
      label: "30+ People",
      desc: "You're a small, but mighty team of curious problem-solvers and explorers. With a versatile, Swiss-knife mentality, we thrive on tackling diverse challenges. Our core team is tight-knit, yet we seamlessly tap into a wider network of experts when needed. Here, theory meets practice, and together, we get things done.",
      img: "https://images.unsplash.com/photo-1438761681033-6461ffad8d80?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "14+ Awards",
      desc: "Our work speaks for itself—recognized internationally, we've already earned some awards. These accolades reflect the passion and innovation we pour into every project, pushing boundaries and delivering results that make an impact.",
      img: "https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "CGN, BLN, Remote",
      desc: "Headquartered in Cologne, with an expanding team in Berlin, we also embrace remote work. Our colleagues span across cities like Barcelona, Stuttgart, Munich, and more, bringing a mix of perspectives and expertise to everything we do. Whether in the office or working remotely, we stay connected and collaborative.",
      img: "https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "B-Corp",
      desc: "We've officially joined the ranks of B-Corp certified companies. This means we meet the highest standards of social and environmental performance, accountability, and transparency. We're proud to use business as a force for good, ensuring our impact extends beyond just profit.",
      img: "https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/B_Corp_Logo.svg/1200px-B_Corp_Logo.svg.png" // Placeholder
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Curious about who we are? Here's a snapshot of the team, our achievements, and the milestones we're proud of.
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
