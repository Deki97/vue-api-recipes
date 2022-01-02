<template>
    <main>
        <div v-if="recipes.length > 0" class="container">
            <Recipe v-for="(item, index) in recipes" :key="index" :objectRecipe="item"/>
        </div>

        <Loader v-else />
    </main>
</template>


<script>
import axios from 'axios';
import Recipe from './Recipe.vue';
import Loader from './Loader.vue';

export default {
    name: 'Main',
    components: {
        Recipe,
        Loader
    },
    data: function() {
        return {
            recipes: []
        };
    },
    created: function() {
        axios.get('https://api.sampleapis.com/recipes/recipes')
        .then((response) => {
            this.recipes = response.data;
        });
    }
}
</script>


<style lang="scss" scoped>

</style>