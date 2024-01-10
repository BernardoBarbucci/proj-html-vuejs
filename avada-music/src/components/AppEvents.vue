<template>
    <section id="sec_title" class="container-fluid">
        <div class="row">
            <div class="offset-4 col-4 pt-4 mb-1 custom_title">
                <h1 class="text-white fw-bold d-flex justify-content-center">Live Dates</h1>
                <hr class="mx-auto custom_hr" />
            </div>
            <div class="offset-3 col-6 text-white text-center mb-3">
                <p id="sec_parag" class="crimson-font">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, fuga veritatis architecto magnificum
                    laudantium
                    oluptatem velit amet?
                </p>
            </div>
        </div>
    </section>

    <!-- events -->
    <section id="events" class="container-fluid">
        <div class="col-10 offset-1">
            <article v-for="(event, index) in events" :key="index" class="col-12 d-flex align-items-center custom_event"
                data-bs-toggle="collapse" :data-bs-target="'#eventCollapse' + index" aria-expanded="false"
                aria-controls="'eventCollapse' + index">
                <p class="mx-2 text-white">+</p>
                <p class="event_name text-uppercase">{{ event.name }}</p>
                <div :id="'eventCollapse' + index" class="collapse custom-collapse" :class="{ 'show': event.expanded }">
                    <p style="height: 10rem;">hello</p>
                </div>
            </article>
        </div>
    </section>

    <!-- latest news -->
    <section class="latestNews d-flex align-items-center justify-content-center">
        <p class="text-black mb-0">VIEW ALL LIVE DATES</p>
    </section>
</template>

<script>
export default {
    name: 'AppEvents',
    data() {
        return {
            events: [
                { name: 'Gem Festival 2024 Anakalia, Georgia', expanded: false },
                { name: 'Groovefest Dominical Republic', expanded: false },
                { name: 'Oasis Festival 2024 Marrakech, Morocco', expanded: false },
                { name: 'Moga Festival - Essaouria, Morocco', expanded: false },
                { name: 'Envision Festival - Uvita, Costa Rica', expanded: false }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import './style/partials/variables.scss';

#sec_title {
    background-color: $bg-color-darkest;
}

#events {
    background-color: $bg-color-darkest;
    padding-bottom: 2rem;

    .custom_event {
        background-color: $bg-color-dark;
        min-height: 2rem;
        margin-bottom: .5rem;
        cursor: pointer;
        transition: height 0.3s linear;

        p {
            margin-bottom: 0;
        }

        .event_name {
            font-size: .75rem;
            color: $theme-color;
        }
    }
}
</style>