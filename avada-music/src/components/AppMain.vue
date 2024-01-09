<template lang="">
    <main>
        <AppMusic />
        <AppNews />
        <AppComment />
        <AppEvents />
    </main>
</template>

<script>
import AppComment from './AppComment.vue';
import AppEvents from './AppEvents.vue';
import AppMusic from './AppMusic.vue';
import AppNews from './AppNews.vue';

export default {
    name: 'AppMain',
    components: {
        AppMain,
        AppComment,
        AppEvents,
        AppNews,
        AppMusic
    }
}
</script>
<style lang="">
    
</style>