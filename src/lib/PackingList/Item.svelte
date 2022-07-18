<script type="ts">
  import Button from "../ui/Button.svelte";

  export let label;
</script>

<Button variant="dark">
  <input type="checkbox" />
  {label}
</Button>
