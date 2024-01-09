<template>
    <section id="sec_title" class="container-fluid">
        <div class="row">
            <div class="offset-4 col-4 pt-3 custom_title">
                <h1 class="text-white fw-bold d-flex justify-content-center">
                    Music is Life
                </h1>
                <hr class="mx-auto custom_hr" />
            </div>
            <div class="offset-3 col-6 text-white text-center mb-3">
                <p id="sec_parag" class="crimson-font">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Magnam, fuga veritatis architecto magnificum laudantium
                    oluptatem velit amet? </p>
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

#sec_title {
    .custom_title {
        border-top: .5rem solid $theme-color;
    }
}
</style>