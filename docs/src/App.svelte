<script>
  import Selector from './Selector.svelte'
  export let colors = [
    'base',
    'box',
    'primary',
    'secondary',
    'info',
    'success',
    'warning',
    'error',
    'highlight',
  ]
</script>

<main class="h-screen bg-base text-base-contrast px-5">
  <section class="mb-24">
    <h1 class="text-6xl text-primary text-center">🦇 Dracula With Tail 🌊</h1>
    <h2 class="text-4xl text-secondary text-center">Awesome tailwind theme</h2>
  </section>

  <!-- Selectors -->
  <section class="flex flex-row items-center justify-center">
    {#each colors as color}
      <Selector variant={color}>{color}</Selector>
    {/each}
  </section>

  <!-- Code -->

</main>
