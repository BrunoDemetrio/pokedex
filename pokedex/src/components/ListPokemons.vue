<script setup>
    const pokemon = defineProps(["name", "url"])
    const idPokemon = pokemon.url.split('/')[6]
    const imageUrl = "https://assets.pokemon.com/assets/cms2/img/pokedex/full/+ idPokemon +.png"
</script>

<template>
    <div class="col-md-4">
        <div class="card mb-3">
            <p class="text-center">{{ pokemon.name }}</p>
            <img src="image" class="card-imf-top" alt="...">
            <div class="card-body">
                <p class="card-title">{{ pokemon.name }}</p>
                <p class="card-title">{{ pokemon.url }}</p>
            </div>
        </div>    
    </div>
</template>

<style>

</style>