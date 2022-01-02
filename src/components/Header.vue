<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/cooking-mama-logo.png" alt="Cooking Mama Logo">
            </div>

            <div class="title">
                <h1>Recipes API</h1>
            </div>
        </div>
    </header>
</template>


<script>
export default {
    name: 'Header'
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

header {
    background-color: $primary-color;
    
    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .logo {
        width: 180px;
    }

    .title {
        color: $secondary-color;

        h1 {
            font-size: 50px;
        }
    }
}
</style>