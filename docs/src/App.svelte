<script>
  import Selector from './Selector.svelte'
  export let colors = [
    'primary',
    'purple',
    'yellow',
    'red',
    'cyan',
    'pink',
    'orange',
    'green',
  ]
</script>

<main class="h-screen bg-base text-base-contrast px-5">
  <section class="mb-24">
    <h1 class="text-6xl text-pink text-center">🦇 Dracula With Tail 🌊</h1>
    <h2 class="text-4xl text-yellow text-center">Awesome tailwind theme</h2>
  </section>

  <!-- Selectors -->
  <section class="flex flex-row items-center justify-center">
    {#each colors as color}
      <Selector variant={color}>{color}</Selector>
    {/each}
  </section>

  <!-- Code -->

</main>
