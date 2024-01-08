<template>
    <header class="container-fluid pt-2">
        <section class="d-flex flex-row justify-content-between px-2">
            <div class="custom_logo">
                <img src="./style/img/avada-music-logo.png" alt="logo">
            </div>
            <div class="custom_menu">
                <i class="fa-solid fa-bars"></i>
            </div>
        </section>
        <section id="hero" class="d-flex flex-column align-items-center">
            <h1 class="fw-bold text-white">
                {{ headerTitle }}
            </h1>
            <h2 class="fst-italic crimson-font">
                <!-- {{ secondaryTitle }} -->
                There is an untold story behind every favorite song.
            </h2>
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
<style lang="scss">
@import './style/partials/variables.scss';

header {
    background-image: url('./style/img/home_slider.jpg');
    background-size: cover;
    background-position: center;
    height: 25rem;
}

.custom_logo img {
    height: 2rem;
    margin-bottom: 5rem;
}

.custom_menu i {
    color: $white;
}

#hero {
    h1 {
        font-size: 3.4rem;
        color: $white;
    }

    h2 {
        font-size: .8rem;
        color: $white;

    }
}
</style>