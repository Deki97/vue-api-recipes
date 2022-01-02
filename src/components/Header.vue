<template>
    <header>
        <div class="logo">
            <img src="../assets/img/cooking-mama-logo.png" alt="Cooking Mama Logo">
        </div>

        <div class="title">
            <h1>Recipes API</h1>
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
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 50px;
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