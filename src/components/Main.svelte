<script lang="ts">
  import Step from "./Step.svelte";

  let steps: any[] = [
    { name: "Smoljames Store", icon: "fa-solid fa-cart-shopping" },
    { name: "Ultimate Todos", icon: "fa-solid fa-list-check" },
    { name: "Pokedex", icon: "fa-solid fa-diagram-project" },
  ];
</script>

<main class="flex flex-col flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl">
        Hi! I'm <span class="poppins text-violet-400">Dan</span> Eyassu <br />
        Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400">favorite tech</span> includes TypeScript,
        JavaScript, Svelte, TailwindCSS & PostgreSQL
      </p>
      <a
        href="#"
        target="_blank"
        class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        ></div>
        <h4 class="relative z-9">Get in touch &rarr;</h4></a
      >
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img
        src={"images/me.jpg"}
        alt="Dan Eyassu"
        class="object-cover z-[2] max-h-[70vh]"
      />
    </div>
  </section>

  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col text-center">
      <h6 class="text-lg sm:text-xl md:text-5xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-violet-400">see</span> my work
      </h3>
    </div>
    <a
      href="https://www.youtube.com/watch?v=-2UjwQzxvBQ"
      target="_blank"
      class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
    >
      <i class="fa-regular fa-circle-play"></i>
      <p>Watch the video</p>
    </a>
    <div>
      <Step step={steps[0]}>
        <p>
          Smoljames Store is a merchandsing store created with <strong
            class="text-violet-400"
            >Next.js Commerces.js Stripe & Node.js + Express.js!</strong
          >Commerce.js is a product CMS and Stripe is used for all transaction
          handling.
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>
          Ultimate Todos is a merchandsing store created with <strong
            class="text-violet-400"
            >Next.js Commerces.js Stripe & Node.js + Express.js!</strong
          >Commerce.js is a product CMS and Stripe is used for all transaction
          handling.
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>
          The Pokedex is a merchandsing store created with <strong
            class="text-violet-400"
            >Next.js Commerces.js Stripe & Node.js + Express.js!</strong
          >Commerce.js is a product CMS and Stripe is used for all transaction
          handling.
        </p>
      </Step>
    </div>
  </section>
</main>
