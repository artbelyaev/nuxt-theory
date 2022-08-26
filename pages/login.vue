<template>
    <form @submit.prevent="onSubmit()">
        <h1>Login</h1>

        <div class="form-group">
            <input type="text" class="form-control mb-2">
        </div>

        <div class="form-group">
            <input type="password" class="form-control mb-2">
        </div>

        <button class="btn btn-primary" type="submit">Login</button>
    </form>
</template>

<script>
export default {
    name: 'login',
    layout: 'login',
    methods: {
        onSubmit() {
            this.$store.dispatch('login');
            this.$router.push('/');
        }
    }
}
</script>

<style scoped>
    form {
        width: 600px;
    }
</style>
