<template>
    <div class="recipe">
        <div class="image">
            <img src="https://plantoeat.s3.amazonaws.com/recipes/16687583/d99596b7acb8758e6d878ada11c36bd83c704cf4-original.jpg?1535321755" alt="Nome Ricetta">
        </div>

        <div class="text">
            <div class="title">
                <h2>California Roll Sushi Bowls</h2>
            </div>

            <div class="ingredients">
                <span>
                    Ingredients:
                </span> 
                2 cups dry California Calrose Sushi Rice\n5 Tbsp rice vinegar, (, divided)\n2 Tbsp granulated sugar\n1/2 tsp salt\n1/4 cup light mayonnaise\n1 1/2 Tbsp sriracha\n1/4 cup low-sodium soy sauce\n10 oz imitation crab, or lump crabmeat, (, torn or chopped into small bite size pieces)\n1 1/2 cups diced English cucumber\n3/4 cup roughly chopped matchstick carrots\n1 nori sheet (, chopped or crumbled into small pieces (add more if you'd like))\n1 1/2 Tbsp chopped pickled sushi ginger\n1 large avocado, (, peeled and diced)\nBlack and toasted sesame seeds, (, for garnish)
            </div>

            <div class="info">
                <div class="preparation-time">
                    <span>
                        Preparation Time:
                    </span> 
                    15 minutes
                </div>
                
                <div class="cooking-time">
                    <span>
                        Cooking Time:
                    </span>
                    25 minutes
                </div>
                
                <div class="total-time">
                    <span>
                        Total Time:
                    </span>
                    40 minutes
                </div>
                
                <div class="servings">
                    <span>
                        Servings:
                    </span>
                    5
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
        min-width: 300px;

        img {
            height: 300px;
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