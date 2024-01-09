<template>
    <section id="sec_title" class="container-fluid">
        <div class="row">
            <div class="offset-3 col-6 pt-4 mb-2 custom_title">
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
    <section id="news" class="container-fluid">
        <div id="cardsWrapper" class="container col-8 offset-2 my_border">

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

// fine sass first section
#news {
    height: 40rem;
    background: $bg-color-darkest;
}

#cardsWrapper {
    height: 95%;
}
</style>