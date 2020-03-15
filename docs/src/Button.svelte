<script>
  export let variant = ''
</script>

<button
  class={`bg-${variant} mr-4 px-6 py-2 text-xl text-primary-faded rounded-sm`}>
  <slot />
</button>
