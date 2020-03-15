<script>
  export let variant = ''
  export let selected = ''
  let isSelected = selected === variant
</script>

<button
  on:click
  class={`bg-${variant} text-${variant}-contrast mr-4 w-32 h-32 text-xl rounded-lg`}>
  <slot />
</button>
