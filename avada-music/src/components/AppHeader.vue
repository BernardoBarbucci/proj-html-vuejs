<template>
    <header class="container-fluid">
        <section class="">
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
            default: 'Untold Stories'
        }
    }
}
</script>
<style lang="">
    
</style>