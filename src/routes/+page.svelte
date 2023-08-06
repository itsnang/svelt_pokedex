<script>
	import { pokemon } from '../stores/pokestore';
	import PokemanCard from '../components/card.svelte';
	console.log($pokemon);
</script>

<svelte:head>
	<title>Pokemon</title>
</svelte:head>
<div class="max-w-5xl mx-auto min-h-screen mt-24 mb-8">
	<div class="grid grid-cols-4 gap-4">
		{#each $pokemon as pokeman}
			<PokemanCard {pokeman} />
		{/each}
	</div>
</div>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}
</style>
