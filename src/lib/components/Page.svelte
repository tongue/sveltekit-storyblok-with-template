<script>
	import { StoryblokComponent } from '@storyblok/svelte';
	export let blok;
</script>

{#if blok}
	<div>
		{#each blok.body as b}
			<StoryblokComponent blok={b} />
		{/each}
	</div>
{/if}
