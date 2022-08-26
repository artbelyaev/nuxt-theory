<template>
    <section>
        <h1>{{ user.name }}</h1>
        <hr>
        <div>{{ user.email }}</div>
    </section>
</template>

<script>
    export default {
        validate({params}) {
            return /^\d+$/.test(params.id);
        },
        async asyncData({params, error, store}) {
            try {
                return await store.dispatch('users/fetchUserById', params.id);
            } catch (e) {
                error(e);
            }
        }
    }
</script>
