<script>
  import { StoryblokComponent } from "@storyblok/svelte";
  export let blok;
</script>

<div>
  {#each blok.columns as column}
    <div>
      <StoryblokComponent blok={column} />
    </div>
  {/each}
</div>
