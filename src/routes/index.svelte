<script>
    import { pokemon } from "../stores/pokestore";
    console.log($pokemon);
</script>
<svelte:head>
    <title>Svelte Kit Pokedex</title>
</svelte:head>
<h1>SvelteKit Pokedex</h1>


{#each $pokemon as pokeman}
<p>
    {pokeman.name}
</p>
{/each}


<style>
    h1 {
        color: red;
    }
</style>
