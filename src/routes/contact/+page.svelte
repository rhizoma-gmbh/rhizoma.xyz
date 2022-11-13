<svelte:head>
  <title>Rhizoma ⸺ Contact</title>
</svelte:head>

<h1 class="text-2xl mb-8">Lets keep in touch!</h1>
<form class="flex flex-col items-stretch gap-5">
  <input class="p-2" placeholder="Full name" type="text" />
  <input class="p-2" placeholder="Mail" type="mail" />
  <textarea
    class="p-2"
    placeholder="Let us know what you want to tell us"
    name="message"
  />
  <div>
    <button
      type="submit"
      class="bg-slate-400 py-3 px-5 text-black hover:text-white hover:bg-black transition-all"
      >Submit</button
    >
  </div>
</form>
