<template>
    <div>
        <header>
            <Navbar />
        </header>
        <main>
            <div class="container">
                <Nuxt />
            </div>
        </main>
    </div>
</template>

<script>
    import Navbar from "@/components/Navbar";

    export default {
        layout: 'default',
        components: {
            Navbar,
        }
    }
</script>

<style scoped>

</style>
