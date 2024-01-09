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
        <div id="cardsWrapper" class="container-fluid col-10 offset-1 d-flex">
            <div id="leftNews" class="col-8 my_border me-2">
                <article class="xCard col-12 mb-3 border">

                </article>
                <div class="d-flex justify-content-between mb-3">
                    <article class="yCard border"></article>
                    <article class="yCard border"></article>
                </div>
                <article class="xCard col-12 border"></article>
            </div>
            <div id="rightNews" class="col-4 d-flex flex-column justify-content-between my_border">
                <article class="yCard col-12 border">
                    <img src="./style/img/blog-post1-200x300.jpg" class="mb-3" alt="mixer">
                    <div class="my_description px-2">
                        <h1 class="mb-1">
                            Taking it back to the old school
                        </h1>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                            Iusto asperiores laudantium debitis voluptas!</p>
                    </div>
                </article>
                <article class="yCard col-12 border"></article>
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

#news {
    height: 50rem;
    background: $bg-color-darkest;
}

#cardsWrapper {
    max-width: 800px;
    margin: auto;

    #leftNews {
        .xCard {
            height: 10rem;
        }

        .yCard {
            height: 20.4rem;
            width: 48%;
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
        font-size: .5rem;
        color: $white;
    }
}
</style>