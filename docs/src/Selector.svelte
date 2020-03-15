<script>
  export let variant = ''
  export let selected = ''
  let isSelected = selected === variant
</script>

<button
  on:click
  class={`bg-${variant} mr-4 w-32 h-32 text-xl text-primary-faded rounded-lg ${isSelected ? 'border-4 border-white' : ''}`}>
  <slot />
</button>
