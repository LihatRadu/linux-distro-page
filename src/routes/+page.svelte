<script>
  import Starback from 'starback';
  import { onMount } from 'svelte';
	import Desktops from '../components/Desktops.svelte';
	import Look from '../components/Look.svelte';

 // const canvas = document.getElementById('canvas');
/**@type {Starback} starback*/
  let starback;

  onMount(() =>{
    starback = new Starback('#canvas',{
        type: 'dot',
        quantity: 100,
        direction: 255,
        backgroundColor: ['#0e1118', '#232b3e'],
        randomOpacity: true,
    });
  }) 

</script>
<section class="bg-gray-900 text-white" id="canvas">
  <div class="mx-auto max-w-screen-xl px-4 py-32 lg:flex lg:h-screen lg:items-center">
    <div class="mx-auto max-w-3xl text-center">
      <h1
        class="bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 bg-clip-text text-3xl font-extrabold text-transparent sm:text-5xl"
      >
        Understand User Flow.

        <span class="sm:block"> Increase Conversion. </span>
      </h1>

      <p class="mx-auto mt-4 max-w-xl sm:text-xl/relaxed">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt illo tenetur fuga ducimus
        numquam ea!
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-4">
        <a
            class="group relative inline-flex items-center overflow-hidden rounded bg-indigo-600 px-8 py-3 text-white focus:outline-none focus:ring active:bg-indigo-500"
            href="/"
>
          <span class="absolute -start-full transition-all group-hover:start-4">
            <svg
              class="size-5 rtl:rotate-180"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M17 8l4 4m0 0l-4 4m4-4H3"
            />
            </svg>
          </span>

          <span class="text-sm font-medium transition-all group-hover:ms-4"> Get Started </span>
        </a>

        <a
          class="block w-full rounded border border-lime-600 px-12 py-3 text-sm font-medium text-white hover:bg-lime-600 focus:outline-none focus:ring active:bg-blue-500 sm:w-auto"
          href="/"
        >
          Learn More
        </a>
      </div>
    </div>
  </div>
</section>

<Desktops/>
<Look/>
