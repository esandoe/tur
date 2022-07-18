<script lang="ts">
  import Heading from "../ui/Heading.svelte";
  import Section from "../ui/Section.svelte";

  let packingList = {
    categories: [
      {
        name: "Søvn",
        items: ["Telt", "Sovepose + liner", "Liggeunderlag", "Pute"],
      },
      {
        name: "Mat",
        items: ["Turmiddag", "Pannekakemiks", "Ketchup", "Pølser", "Pølsebrød"],
      },
      {
        name: "Snacks",
        items: ["Kvikk Lunsj", "Nøtteblanding", "Seigmenn"],
      },
      {
        name: "Klær",
        items: [
          "Ullgenser",
          "Vindtett/vannavstøtende jakke",
          "Ullsokker",
          "T-skjorte",
          "Turshorts",
        ],
      },
    ],
  };
</script>

<Section>
  <Heading size="lg">Pakkeliste</Heading>

  <div style="display: flex; flex-direction: column; gap: 1em;">
    {#each packingList.categories as category}
      <Heading size="sm">{category.name}</Heading>
      {#each category.items as item}
        <label>
          <input type="checkbox" />
          {item}
        </label>
      {/each}
    {/each}
  </div>
</Section>
