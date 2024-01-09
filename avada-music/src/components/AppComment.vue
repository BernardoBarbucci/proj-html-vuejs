<template>
    <section class="container-fluid py-5">
        <div id="custom_comment" class="col-6 offset-3 my_border mb-3">
            <p class="crimson-font fst-italic text-center">
                "I just listened to it and said to myself, "Man, I really love this album." Still, todaym it just sounds so
                fresh. It sounds full of ideas.
                These guys knew what they were doing. They're good. And they're inventive. I haven't heard anything this
                year that's as inventive. I don't really expect to."
            </p>
            <img src="./style/img/band_interview_play_icon.png" alt="play">
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppComment',
}
</script>

<style lang="scss" scoped>
section {
    background-image: url('./style/img/home-testimonial-parallax.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

#custom_comment {}
</style>