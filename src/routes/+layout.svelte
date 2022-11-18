<script>
  import Plausible from "plausible-tracker";
  import { browser } from "$app/environment";
  import "../app.css";

  if (browser) {
    const plausible = Plausible({
      domain: "rhizoma.dev",
    });

    plausible.enableAutoPageviews();
  }
</script>

<div class="flex flex-col min-h-screen">
  <img
    class="absolute -top-40 right-0 opacity-40"
    src="./images/header_misc.svg"
    alt="Decoration"
  />
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
      </nav>
    </div>
  </header>
  <main class="w-full flex-1 md:mx-auto py-4 pt-16 px-5">
    <slot />
  </main>
  <footer class="container mx-auto flex items-end justify-between opacity-40">
    <img src="./images/footer_misc.svg" alt="Decoration" />
    <span class="hidden md:inline text-xs mb-4">Designed by Rhizoma GmbH</span>
  </footer>
</div>
