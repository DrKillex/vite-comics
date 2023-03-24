<script>
import { stringifyExpression } from '@vue/compiler-core';

export default {
    name: "Card",
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div class="img"><img :src="img"></div>
        <h3>{{ title }}</h3>
    </div>
</template>

<style scoped lang="scss">

</style>