<template>
    <section id="sec_title" class="container-fluid">
        <div class="row">
            <div class="offset-3 col-6 pt-4 mb-3 custom_title my_border">
                <h1 class="text-white fw-bold d-flex justify-content-center">
                    Latest Band News
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
    name: 'AppNews',
}
</script>

<style lang="scss" scoped>
@import './style/partials/variables.scss';

#sec_title {
    background-color: $bg-color-darkest;

}
</style>