<template>
    <main>
        <div class="container">
            <Recipe />
            <Recipe />
            <Recipe />
            <Recipe />
            <Recipe />
            <Recipe />
        </div>
    </main>
</template>


<script>
import axios from 'axios';
import Recipe from './Recipe.vue';

export default {
    name: 'Main',
    components: {
        Recipe
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