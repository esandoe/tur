<script lang="ts">
  import Item from "./Item.svelte";

  let items: string[] = ["Telt", "Sovepose"];
</script>

<div style="display: flex; flex-direction: column; gap: 1em;">
  {#each items as item}
    <Item label={item} />
  {/each}
</div>
