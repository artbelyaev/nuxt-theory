<template>
    <section>
        <h1>Users page</h1>
        <ul>
            <li v-for="user in users">{{ user }}</li>
        </ul>
    </section>
</template>

<script>
export default {
    name: `users`,
    data() {
        return {
            users: [
                1, 2, 3, 4, 5
            ]
        }
    }
}
</script>

<style scoped>

</style>
