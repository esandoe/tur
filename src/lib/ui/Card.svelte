<script lang="ts">
  export let variant: string = "light";
</script>

<div
  style:border-radius="8px"
  style:margin-block="18px"
  style:padding="18px 28px"
  class={"card " + variant}
>
  <slot />
</div>

<style>
  .card {
    color: var(--light);
  }

  .light {
    background-color: var(--light);
    color: var(--dark);
  }
  .dark {
    background-color: var(--dark);
  }
  .accent {
    background-color: var(--dark-accent);
  }
  .sky {
    background: linear-gradient(
      27deg,
      rgba(254, 215, 148, 1) 0%,
      rgba(186, 129, 197, 1) 46%,
      rgb(40, 36, 90) 100%
    );
  }
</style>
