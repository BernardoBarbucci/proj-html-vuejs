<template>
    <section id="music_life" class="container-fluid">
        <div class="row">
            <div class="offset-4 col-4 pt-3 custom_title">
                <h1 class="text-white fw-bold d-flex justify-content-center">
                    Music is Life
                </h1>
                <hr class="mx-auto" />
            </div>
            <div class="offset-3 col-6 text-white text-center mb-3">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, fuga veritatis architecto magni
                    laudantium voluptatem velit amet? </p>
            </div>
        </div>

    </section>
</template>
<script>
export default {
    name: 'AppMusic',
}
</script>
<style lang="scss" scoped>
@import './style/partials/variables.scss';

section {
    background-color: $bg-color-dark;

    .custom_title {
        height: 6rem;
        border-top: .5rem solid $theme-color;

        h1 {
            font-size: 2.2rem;
        }
    }
}

hr {
    color: $white;
    width: 9rem;
}

p {
    font-size: .65rem;
    color: $p-text;
}
</style>