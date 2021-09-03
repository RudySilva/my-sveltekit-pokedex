<script>
    import { pokemon } from "../stores/pokestore";
    import PokemanCard from "../components/PokemanCard.svelte";
    //console.log($pokemon);
</script>
<svelte:head>
    <title>Svelte Kit Pokedex</title>
</svelte:head>
<h1 class="text-2xl text-center my-8 uppercase">SvelteKit Pokedex</h1>

<div class="py-4 grid gap-4 md:grid-cols-2 grid-cols-1">
    {#each $pokemon as pokeman}
    <PokemanCard pokeman={pokeman} />
    {/each}
</div>



<style>
    h1 {
        color: red;
    }
</style>
