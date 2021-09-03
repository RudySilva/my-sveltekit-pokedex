<script>
    import { pokemon } from "../stores/pokestore";
    import PokemanCard from "src/components/pokemanCard.svelte";
    //console.log($pokemon);
</script>
<svelte:head>
    <title>Svelte Kit Pokedex</title>
</svelte:head>
<h1 class="text-2xl text-center my-8 uppercase">SvelteKit Pokedex</h1>


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
