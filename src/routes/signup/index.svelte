<script>
import Link from "../../components/ExternalLink.svelte";

  let isClosed = true;

  let isLoaded = false;
  let cannotLoad = false;
  let formHeight = 0;

  function changeLoad() {
    isLoaded = true;
  }

  function neverLoaded() {
    if (!isLoaded) cannotLoad = true;
    isLoaded = true;
    formHeight = 2000; 
  }

  setTimeout(neverLoaded, 2000)

</script>

<div class="text-center text-3xl md:text-4xl lg:text-5xl font-medium mt-16 mb-16">Sign up here!</div>
<div>

  {#if isClosed}
    <div class="text-center text-xl md:text-2xl lg:text-3xl text-red-600">
      Classes are closed.
    </div>
  {:else} 
  

  <div class="text-center text-lg md:text-xl lg:text-2xl mb-4">
    If the signup form does not load, <Link href="https://forms.gle/3eX76gKarDvzKYm8A" text="click here"/> to fill out the form.
  </div>
  
  {#if !isLoaded}
    <div class="text-center text-xl md:text-2xl lg:text-3xl text-gray-600">
      Loading...
    </div>
  {/if}
  {#if !cannotLoad}
    <div class="flex justify-center">
      <iframe class="w-full" on:load={changeLoad} height={formHeight} src="https://docs.google.com/forms/d/e/1FAIpQLSe9A67R4pRumX-lqRYpChZMyeLC9t6zwDXHP_t0I7UvMKWQFA/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0" title="Signup Form">Loading…</iframe>
    </div>
  {:else}
    <div class="text-center text-xl md:text-2xl lg:text-3xl text-red-600">
      Sorry, could not load signup form.
    </div>
  {/if}
  {/if}
</div>
