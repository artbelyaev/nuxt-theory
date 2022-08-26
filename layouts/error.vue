<template>
    <section>
        <h1>Error 404</h1>
        <NuxtLink to="/">Home</NuxtLink>
    </section>
</template>

<script>
export default {
    name: "error"
}
</script>

<style scoped>
    h1 {
        color: red;
    }

    section {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>
