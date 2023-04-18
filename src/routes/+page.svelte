<script>
  import { StoryblokComponent } from "@storyblok/svelte";

  export let data;
</script>

<div>
  {#if data.story}
    <StoryblokComponent blok={data.story.content} />
  {/if}
</div>
