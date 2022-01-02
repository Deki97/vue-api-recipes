<template>
    <div class="recipe">
        <div class="image">
            <img :src="objectRecipe.photoUrl" :alt="objectRecipe.title">
        </div>

        <div class="text">
            <div class="title">
                <h2>{{ objectRecipe.title }}</h2>
            </div>

            <div class="ingredients">
                <span>
                    Ingredients:
                </span> 
                {{ objectRecipe.ingredients }}
            </div>

            <div class="info">
                <div class="preparation-time">
                    <span>
                        Preparation Time:
                    </span> 
                    {{ objectRecipe.prepTime}}
                </div>
                
                <div class="cooking-time">
                    <span>
                        Cooking Time:
                    </span>
                    {{ objectRecipe.cookTime }}
                </div>
                
                <div class="total-time">
                    <span>
                        Total Time:
                    </span>
                    {{ objectRecipe.totalTime }}
                </div>
                
                <div class="servings">
                    <span>
                        Servings:
                    </span>
                    {{ objectRecipe.servings }}
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Recipe',
    props: {
        objectRecipe: Object
    }
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

.recipe {
    display: flex;
    margin: 20px 0;

    .image {
        min-width: 280px;

        img {
            height: 280px;
            object-fit: cover;
            object-position: center;
            cursor: pointer;
        }
    }

    .text {
        margin-left: 30px;
        font-size: 24px;

        .title {
            color: $secondary-color;
            cursor: pointer;
            display: inline-block;

            h2 {
                font-size: 36px;
            }
        }
    }

    .info {
        display: flex;
        margin-top: 20px;

        div {
            margin-right: 20px;
        }
    }

    & span {
        color: $primary-color;
        font-weight: bold;
    }
}
</style>