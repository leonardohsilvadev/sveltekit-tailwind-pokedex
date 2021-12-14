<script>
	import { pokemon } from '../stores/pokestore';
	console.log($pokemon);
</script>

<svelte:head>
	<title>Pokedex</title>
</svelte:head>

<h1>Index</h1>

{#each $pokemon as p}
	<p>{p.name}</p>
{/each}

<style>
	h1 {
		color: red;
	}
</style>
