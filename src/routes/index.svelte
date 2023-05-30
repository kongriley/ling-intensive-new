<script>
  import ExternalLink from '../components/ExternalLink.svelte'
  import ClassButton from '../components/ClassButton.svelte'
</script>

<div class="md:hero-height md:min-h-0 bg-gradient-to-b from-indigo-100 to-white">
  <div class="relative mx-auto max-w-screen-xl pt-12 md:pt-16 lg:pt-20 px-6 lg:px-16 xl:pt-28">
    <div class="sm:text-center lg:text-left">
      <div class="text-4xl tracking-tight leading-10 font-semibold text-gray-900 sm:text-5xl sm:leading-none md:text-6xl">
        Welcome to the 
        <br>
        Linguistics Intensive!
      </div>
      <p class="mt-3 text-base text-gray-600 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0">
        Spreading the joy of logic and linguistics to aspiring linguists. Run by students, for students.
      </p>
    </div>
  </div>
</div>

<div class="flex justify-center">

  <div class="text-md md:text-lg lg:text-xl mx-8 md:mx-24 lg:mx-40 xl:w-1/2 text-gray-600">

    <div class="text-center text-2xl md:text-3xl lg:text-4xl font-medium mb-6 mt-20 text-black">
      What is LINT?
    </div>

    <div>
      The <span class="font-bold">Lin</span>guistics <span class="font-bold">Int</span>ensive (LINT, pronounced /lɪnt/) 
      aims to bring linguistics and logical thinking to a wider audience.
      We recognize that linguistics is often overlooked in the school curriculum and as an academic field;
      virtually no schools offer classes in linguistics, and there is a lack of resources accessible to younger students.
      As such, we strive to provide free, high-quality education in linguistics to expand this field to the next generation.
    </div>
    
    <div class="text-center text-2xl md:text-3xl lg:text-4xl font-medium mt-20 mb-6 text-black">
      Programs at LINT
    </div>

    <div>
      LINT offers online courses designed to prepare students in 7th to 12th grade for the
      <ExternalLink href="https://www.nacloweb.org/" text="NACLO" /> 
      (North American Computational Linguistics Open competition) and the
      <ExternalLink href="https://ioling.org/" text="IOL" /> 
      (International Linguistics Olympiad). 
      Students will investigate features of world languages, including grammar, phonetics, number systems, and writing systems, 
      along with topics in computational linguistics and analytic reasoning.
    </div>
    

    <div class="mt-20 flex lg:flex-shrink-0 justify-center items-center">
      <div class="text-xl md:text-2xl lg:text-3xl font-medium mr-6">Ready?</div>
      <ClassButton />
    </div>
  </div>
</div>