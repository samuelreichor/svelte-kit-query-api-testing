<script lang="ts">
	import CraftMatrix from '$lib/components/CraftMatrix.svelte';
	import type { CraftPageHome } from '../../queryApiTypes';
	import RelatedNews from '../blocks/RelatedNews.svelte';

	const homeProps = $props() as CraftPageHome;
</script>

<div>
	<h1>{homeProps.title}</h1>

	{#if homeProps.contentBuilder}
		<CraftMatrix content={homeProps.contentBuilder} />
	{/if}

	<RelatedNews />
</div>
