<script lang="ts">
	export let child = false;
	export let n: number;
</script>

<p>{n}</p>

{#if child}
	<!-- replacing svelte:self with svelte:component and importing the component itself works as expected -->
	<svelte:self n="this should not be valid" />
{/if}
