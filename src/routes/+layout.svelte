<script>
  import "../app.css";

  export const prerender = true;
</script>

<div class="flex flex-col min-h-screen">
  <header
    class="md:container md:mx-auto mx-5 my-10 flex justify-between items-center"
  >
    <a href="/">
      <div class="flex items-center">
        <img src="./images/logo.svg" alt="Radicle Logo" />
        <span class="inline-block ml-2 text-xl">Rhizoma</span>
      </div>
    </a>
    <div>
      <nav class="relative flex items-center gap-8">
        <a class="z-10" href="/team">team</a>
        <a class="z-10" href="/clients">clients</a>
        <a class="z-10" href="/contact">contact</a>
        <img
          class="absolute z-0 -right-12 -top-60 max-w-none opacity-40"
          src="./images/header_misc.svg"
          alt="Decoration"
        />
      </nav>
    </div>
  </header>
  <main class="container flex-1 md:mx-auto my-4 mt-16 mx-5">
    <slot />
  </main>
  <footer class="container mx-auto flex items-end justify-between opacity-40">
    <img src="./images/footer_misc.svg" alt="Decoration" />
    <span class="hidden md:inline text-xs mb-4">Designed by Rhizoma GmbH</span>
  </footer>
</div>
