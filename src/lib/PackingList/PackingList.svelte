<script lang="ts">
  import Heading from "../ui/Heading.svelte";
  import Section from "../ui/Section.svelte";
  import Item from "./Item.svelte";

  let items: string[] = ["Telt", "Sovepose"];
</script>

<Section>
  <Heading size="lg">Pakkeliste</Heading>

  <div style="display: flex; flex-direction: column; gap: 1em;">
    {#each items as item}
      <Item label={item} />
    {/each}
  </div>
</Section>
