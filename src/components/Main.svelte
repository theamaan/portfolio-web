<script>
  import Step from "./Step.svelte";

  let steps = [
    {
      name: "CeleriHire: Dynamic Employee Management",
      icon: "fa-solid fa-cart-shopping",
      description:
        "Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
    },
    {
      name: "Ticket Booking Application",
      icon: "fa-solid fa-list-check",
      description:
        "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
    },
    {
      name: "ICODING: A BLOGGING WEBSITE",
      icon: "fa-solid fa-diagram-project",
      description:
        " your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
    },
  ];

  let benefits = [
    {
      metric: "10x",
      name: "a self taught developer",
      description:
        "My coding journey commenced with a strong foundation in Java, a programming language renowned for its robustness and versatility. Subsequently, I delved into the dynamic realm of web development, immersing myself in the intricacies of JavaScript, HTML, and CSS. My dedication to this craft led me to explore a wide spectrum of skills, encompassing JavaScript frameworks, backend programming, design principles, as well as the integration of cloud services, and a myriad of other advanced concepts.",
    },
    {
      name: "expanding horizons",
      description:
        "Beyond the confines of coding, I am an avid learner. My dedication to improving my vocabulary goes hand in hand with my quest for coding mastery. In the ever-evolving world of technology, communication skills are paramount, and I believe in achieving eloquence both in code and in words.",
    },
    {
      name: "my professional aspirations:",
      description:
        "My dedication extends beyond skill refinement. I am actively seeking opportunities in the fields of Full Stack and Backend Development, aspiring to contribute my expertise and creativity to innovative projects.",
    },
    {
      name: "a touch of humor",
      description:
        "While I'm deeply immersed in the world of technology, I also embrace the lighter side of life. Memes, with their witty humor, are a delightful part of my daily routine. They serve as a reminder that even in the most serious of endeavors, a touch of humor can go a long way.",
    },
  ];
</script>

<main class="flex flex-col flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-violet-400">Amaan</span> Ullah
        <br />Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400"> favorite tech</span> includes Java, Spring
        Boot (React.JS or SvelteKit), TailwindCSS, Node.js + JavaScript & PostgreSQL
        or MySQL!
      </p>
      <button
        class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <a href="https://twitter.com/theamaan13" class="relative z-9"
          ><h4>Get in touch &rarr;</h4></a
        >
      </button>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img
        src={"images/IMG_5005.jpeg"}
        alt="Amaan's Pic"
        class="object-cover z-[2] max-h-[70vh]"
      />
    </div>
    <!-- <div  class="flex p-0.5 relative max-w-[700px] w-full mx-auto">
            <div
                class="absolute inset-0 overflow-hidden rounded-md flex items-center justify-center"
            >
                <div
                    class="bg-gradient-to-r absolute inset-[-20px]  from-violet-800 to-indigo-800 specialSpin"
                />
            </div>

            <img
                src={"images/zetane-engine.jpeg"}
                alt="Zetane Engine"
                class="w-full h-full object-cover z-[2]"
            />
        </div> -->
  </section>
  <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-large sm:text-xl md:text-2xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-violet-400">see</span> my work?
      </h3>
    </div>
    <!-- <a
      href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
      target="_blank"
      class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
    >
      <i class="fa-regular fa-circle-play" />
      <p>Watch the video</p>
    </a> -->
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>
          CeleriHire is a meticulously crafted, user-centric software solution
          engineered with precision and created with <strong
            class="text-violet-400"
            >React.js, Spring Boot, MySQL & Bootstrap + Postman</strong
          >. We Prioritized user experience (UX) principles for an intuitive and
          aesthetically pleasing interface.
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>
          Developed the application using the
          <!-- <strong class="text-violet-400">Next.js</strong>, -->
          <strong class="text-violet-400">Golang</strong>
          <!-- & <strong class="text-violet-400">Firebase</strong>  -->
          renowned for its efficiency and robustness in software engineering.
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>
          Construct the website utilizing the <strong class="text-violet-400"
            >Bootstrap Framework</strong
          >
          ,renowned for its exceptional capabilities in facilitating responsive and
          visually appealing web development, crafted using a blend of
          <strong class="text-violet-400"> HTML, CSS and JavaScript</strong>.
          <!-- <strong class="text-violet-400">Pokémon API</strong> -->
        </p>
      </Step>
    </div>
  </section>
  <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
  >
    <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
    <div
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h6 class="text-large sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        A bit <span class="poppins text-violet-400">about</span> me.
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am . . .
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
        <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
        <div class="flex gap-6 sm:gap-8">
          <p
            class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
          >
            0{index + 1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <p>{benefit.description}</p>
          </div>
        </div>
      {/each}
    </div>
    <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
      The <span class="text-violet-400">Complete</span> Package
    </h5>
    <div
      class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
    >
      <table class="bg-white text-slate-700 rounded text-center">
        <thead class={"border-b border-solid border-slate-200  "}>
          <tr class="">
            <th />
            <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
            <th class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
              >Me</th
            >
          </tr>
        </thead>
        <tbody>
          <tr class="border-b border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Dedication</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Critical Thought</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr>
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              > Adaptability</td
            >
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr class="border-t border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Coding Practices</td
            >
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr class="border-t border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Problem Solving</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
      <p>Scroll to see more &rarr;</p>
    </div>
    <p class="mx-auto">So why not invest?</p>
  </section>
</main>
