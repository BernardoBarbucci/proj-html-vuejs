<template>
    <section id="sec_title" class="container-fluid">
        <div class="row">
            <div class="offset-3 col-6 pt-4 mb-1 custom_title">
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
        <div id="cardsWrapper" class="container-fluid col-10 offset-1 d-flex">
            <div id="leftNews" class="col-8 me-2">
                <article class="xCard col-12 mb-3">
                    <img src="./style/img/blog_music_techo-1200x600.jpg" class="mb-2" alt="mixer">
                    <div class="my_description px-2 pt-2">
                        <h1 class="mb-1">
                            Technology and Music
                        </h1>
                        <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                            Iusto asperiores laudantium debitis voluptas!</p>
                    </div>
                </article>
                <div class="d-flex justify-content-between mb-3">
                    <article class="yCard">
                        <img src="./style/img/blog-post3-600x900.jpg" class="mb-2" alt="guitars">
                        <div class="my_description px-2">
                            <h1 class="mb-1">
                                While my guitar gently weeps
                            </h1>
                            <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                                Iusto asperiores laudantium debitis voluptas!</p>
                        </div>
                    </article>
                    <article class="yCard">
                        <img src="./style/img/blog-post4-600x900.jpg" class="mb-2" alt="vynils">
                        <div class="my_description px-2">
                            <h1 class="mb-1">
                                It just sounds better
                            </h1>
                            <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                                Iusto asperiores laudantium debitis voluptas!</p>
                        </div>
                    </article>
                </div>
                <article class="xCard col-12">
                    <img src="./style/img/blog_flavor_rock-600x300.jpg" class="mb-2" alt="rocker">
                    <div class="my_description px-2 pt-2">
                        <h1 class="mb-1">
                            The flavor of rock
                        </h1>
                        <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                            Iusto asperiores laudantium debitis voluptas!</p>
                    </div>

                </article>
            </div>
            <div id="rightNews" class="col-4 d-flex flex-column justify-content-between">
                <article class="yCard col-12">
                    <img src="./style/img/blog-post1-600x900.jpg" class="mb-2" alt="night street">
                    <div class="my_description px-2">
                        <h1 class="mb-1">
                            Taking it back to the old school
                        </h1>
                        <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                            Iusto asperiores laudantium debitis voluptas!</p>
                    </div>
                </article>
                <article class="yCard col-12">
                    <img src="./style/img/blog-post2-600x900.jpg" class="mb-2" alt="guitarist">
                    <div class="my_description px-2">
                        <h1 class="mb-1">
                            Sharing the stage with a legend
                        </h1>
                        <p class="crimson-font">Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                            Iusto asperiores laudantium debitis voluptas!</p>
                    </div>
                </article>
            </div>
        </div>
    </section>
    <section class="latestNews d-flex align-items-center justify-content-center">
        <p class="text-black mb-0">
            VIEW ALL THE LATEST NEWS
        </p>
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

#news {
    padding-bottom: 4rem;
    background: $bg-color-darkest;
}

#cardsWrapper {
    max-width: 750px;
    min-width: 560px;
    margin: auto;

    #leftNews {
        .xCard {
            position: relative;
            height: 10rem;

            &:hover .my_description {
                display: none;
            }

            img {
                width: 100%;
                height: 100%;

                &:hover {
                    opacity: 0.7;
                    filter: rgba(236, 72, 88, 0.8);
                }
            }

            .my_description {
                min-height: 53.41px;
                padding-top: .3rem;
                position: absolute;
                bottom: 0;
                width: 100%;
                background-color: $bg-color-dark;

                p {
                    margin-bottom: .3rem;
                }
            }
        }

        .yCard {
            height: 20.4rem;
            width: 48%;
            // position: relative;

            // &:hover .my_description {
            //     display: none;
            // }

            img {
                height: 80%;
                width: 100%;
            }

            // .my_description {
            //     position: absolute;
            // }
        }
    }

    #rightNews {
        .yCard {
            height: 20.7rem;

            img {
                height: 80%;
                width: 100%;
            }
        }
    }
}

article {
    background-color: $bg-color-dark;
}

.my_description {
    h1 {
        font-size: .7rem;
        font-weight: bold;
        color: $theme-color;
    }

    p {
        font-size: .55rem;
        font-weight: bold;
        color: $p-text;
    }
}
</style>