<template>
    <section id="music_life" class="container-fluid">
        <div class="row">
            <div class="offset-4 col-4 border">
                <h1 class="text-white fw-bold d-flex justify-content-center">
                    Music if Life
                </h1>
                <hr />
            </div>
            <div class="offset-3 col-6 text-white">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, fuga veritatis architecto magni
                    laudantium
                    voluptatem velit amet? Tempora perspiciatis, deserunt reprehenderit ex natus aut corrupti. Reprehenderit
                    placeat sed facere. Velit?</p>
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
    height: 15rem;
}

hr {
    color: $white;
    width: 3rem;
}
</style>