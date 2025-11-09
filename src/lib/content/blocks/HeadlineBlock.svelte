<script lang="ts">
	import type { CraftEntryTypeHeadline } from '../../queryApiTypes';

	const headlineProps = $props() as CraftEntryTypeHeadline;
	const tag = headlineProps.headlineTag.value;
	const headline = headlineProps.title;
</script>

<svelte:element this={tag}>
	{headline}
</svelte:element>
