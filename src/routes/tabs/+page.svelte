<script lang="ts">
  let tabSet: number = 0;
  import { TabGroup, Tab } from "@skeletonlabs/skeleton";
</script>

<div class="card variant-glass p-4 space-y-4">
  Hello mj!!
  <TabGroup>
    <Tab bind:group={tabSet} name="tab1" value={0}>books</Tab>
    <Tab bind:group={tabSet} name="tab2" value={1}>movies</Tab>
    <Tab bind:group={tabSet} name="tab3" value={2}>tv</Tab>
    <svelte:fragment slot="panel">
      {#if tabSet === 0}
        <p>A written or printed work</p>
      {:else if tabSet === 1}
        <p>A story or event recorded by a camera</p>
      {:else if tabSet === 2}
        <p>A system for transmitting moving imagesv</p>
      {/if}
    </svelte:fragment>
  </TabGroup>
</div>
