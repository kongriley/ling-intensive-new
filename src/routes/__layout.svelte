<script>
  import "../app.css";
  import ExternalLink from '../components/ExternalLink.svelte'
</script>

<div class="sticky top-0 flex flex-wrap items-baseline justify-between md:justify-start px-6 md:px-16 bg-indigo-100 z-10 p-4 pb-5">
  <div class="flex-none mr-8 text-lg md:text-xl font-semibold">
    <a href="/">
      LINT
    </a>
  </div>
  <div class="flex items-center ">
    <a href="/" class="text-gray-900 hover:text-gray-700 transition duration-300 ease-in-out">
      home
    </a>
    ・
    <a href="classes" class="text-gray-900 hover:text-gray-700 transition duration-300 ease-in-out">
      classes
    </a>
    ・
    <a href="instructors" class="text-gray-900 hover:text-gray-700 transition duration-300 ease-in-out">
      instructors
    </a>
    ・
    <a href="signup" class="font-medium text-indigo-600 hover:text-indigo-500 transition duration-300 ease-in-out">
      signup
    </a>
  </div>
</div>

<slot />

<div class="flex justify-center">
  <div class="grid grid-cols-1 divide-x-2 text-center footer mt-16 md:mt-24 mb-10 md:mb-14 w-2/3 text-sm md:text-md lg:text-lg">
    <div>
      <ExternalLink href="mailto:lingintensive@gmail.com" class="text-indigo-600 hover:text-indigo-800" text="Questions? Contact LINT via email here" />
    </div>
  </div>
</div>