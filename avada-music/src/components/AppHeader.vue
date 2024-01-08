<template>
    <header class="container-fluid">
        <section>
            <h1 class="fw-bold">
                {{ headerTitle }}
            </h1>
        </section>
    </header>
</template>
<script>
export default {
    name: 'AppHeader',
    props: {
        headerTitle: {
            type: String,
            default: 'Default title'
        }
    }
}
</script>
<style lang="">
    
</style>