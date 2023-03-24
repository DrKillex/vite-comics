<script>
import CardSection from './CardSection.vue';

export default {
    name: "AppMain",
    components: {
        CardSection
    }
    }
</script>

<template>
    <main>
        <CardSection></CardSection>
    </main>   
</template>

<style scoped lang="scss">
main {
    background-image: url(src/assets/img/jumbotron.jpg);
    background-position: center;
    background-size: cover;
    display: flex;
    align-items: flex-end;
    padding-top: 500px;
}
</style>