<template>
    <AppHeader :headerTitle="headerMainTitle" :secondaryTitle="headerSecondaryTitle" />
    <Appmain>
        <AppMusic />
        <AppNews />
        <AppComment />
        <AppEvents />
    </Appmain>
    <AppFooter />
</template>

<script>
import AppMain from './components/AppMain.vue';
import AppComment from './components/AppComment.vue';
import AppEvents from './components/AppEvents.vue';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMusic from './components/AppMusic.vue';
import AppNews from './components/AppNews.vue';

export default {
    name: 'App',
    components: {
        AppHeader,
        AppMain,
        AppComment,
        AppEvents,
        AppNews,
        AppMusic,
        AppFooter
    },
    data() {
        return {
            headerMainTitle: 'Untold Stories',
            headerSecondaryTitle: 'There is an untold story behind every favorite song.',
        };
    }
}
</script>

<style lang="scss">
@use './components/style/main.scss' as *;
@use './components/style/partials/variables.scss' as *;

// * {
//     background-color: $bg-color-darkest;
// }
</style>


<!-- enter term
cd C:\Users\berna\OneDrive\Desktop\proj-html-vuejs\avada-music
-->