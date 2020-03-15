<script>
  import Button from './Button.svelte'
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
  <ul>
    {#each colors as color}
      <li class={`text-${color} text-5xl`}>{color}</li>
    {/each}
  </ul>
  <section>
    <h1 class="text-5xl text-pink">Buttons example</h1>
    {#each colors as color}
      <Button variant={color}>{color}</Button>
    {/each}
  </section>
</main>
