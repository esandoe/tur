<script lang="ts">
  export let size: string = "sm";

  const HeadingTypes = {
    sm: "h4",
    md: "h3",
    lg: "h2",
  };
</script>

<svelte:element this={HeadingTypes[size]} class="header-{size}">
  <slot />
</svelte:element>

<style>
  .header-sm,
  .header-md {
    margin-block: 15px 6px;
  }

  .header-lg {
    margin-block: 15px;
  }
</style>
