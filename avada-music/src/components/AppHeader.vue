<template>
    <header class="container-fluid pt-2">

        <section class="d-flex flex-row justify-content-between px-3 top-section">
            <div class="custom_logo">
                <img src="./style/img/avada-music-logo.png" alt="logo">
            </div>
            <div class="custom_menu" @click="toggleMenu">
                <i class="fa-solid fa-bars"></i>
            </div>
        </section>

        <!-- Menu da mostrare -->
        <ul v-if="showMenu" class="menu-overlay pt-2">
            <section class="d-flex flex-row justify-content-between top-section">
                <div class="custom_logo">
                    <img src="./style/img/avada-music-logo.png" alt="logo">
                </div>
                <div class="custom_menu" @click="toggleMenu">
                    <i class="fa-solid fa-xmark"></i>
                </div>
            </section>
            <!-- menu list onclick -->
            <li v-for="item in menuItems" :key="item">{{ item }}</li>
        </ul>

        <section id="hero" class="d-flex flex-column align-items-center">
            <h1 class="fw-bold text-white">
                {{ headerTitle }}
            </h1>
            <h2 class="fst-italic crimson-font mb-4">
                {{ secondaryTitle }}
            </h2>
            <div class="my_buttons d-flex justify-content-between">
                <button type="button"
                    class="custom_button text-white d-flex justify-content-center align-items-center">LATEST ALBUM</button>
                <button type="button" class="btn btn-outline-light d-flex justify-content-center align-items-center">LIVE
                    DATES</button>
            </div>
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
        },
        secondaryTitle: {
            type: String,
            default: 'Default secondary title'
        },
        // menu logic
        menuItems: {
            type: Array,
            // parte sotto sostituibile anche con un arrow function, basta che restituisca una function senza argomenti
            default: function () {
                return [];
            }
        }
    },
    data() {
        return {
            showMenu: false,
        };
    },
    // richiamo la function con methods
    methods: {
        toggleMenu() {
            // cambia il valore di showMenu nel componente
            this.showMenu = !this.showMenu;
        }
    },
}
</script>

<style lang="scss" scoped>
@import './style/partials/variables.scss';

header {
    background-image: url('./style/img/home_slider.jpg');
    background-size: cover;
    background-position: center;

}

.top-section {

    .custom_logo img {
        height: 2rem;
        margin-bottom: 5rem;
    }

    .custom_menu i {
        color: $white;
    }
}

#hero {
    height: 17.5rem;

    h1 {
        font-size: 4rem;
    }

    h2 {
        font-size: .8rem;
        color: $white;
    }
}

.my_buttons {
    width: 12.5rem;

    button {
        height: 1.5rem;
        border-radius: 2px;
        width: 6rem;
        font-size: .7rem;
    }

    .custom_button {
        background-color: $theme-color;
        border: none;
        transition: linear .18s;
    }

    .custom_button:hover {
        background-color: black;
        color: $white;
    }
}

// toggleMenu sass

.menu-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 400px;
    background-color: #ec4858;
    display: flex;
    flex-direction: column;
    align-items: center;
    list-style-type: none;
    padding: 0;
    margin: 0;
    color: white;
    font-size: 1.2rem;
}

.menu-overlay li {
    margin-bottom: 1rem;
    cursor: pointer;
}

ul {

    .top-section {
        padding-left: 1.5rem;
        padding-right: 1.5rem;
        width: 100%;
    }
}
</style>