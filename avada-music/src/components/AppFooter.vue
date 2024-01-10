<template>
    <footer>
        <section id="footerMenu" class="col-12 d-flex align-items-center justify-content-between">
            <div class="footerLogo">
                <img src="./style/img/logo_footer.png" alt="logo footer">
            </div>
            <div class="footerInfos">
                <ul class="d-flex flex-row">
                    <li v-for="(menuItem, index) in menuItems" :key="index">
                        {{ menuItem }}
                    </li>
                </ul>
            </div>
        </section>
        <section id="copyright" class="col-12 d-flex align-items-center justify-content-between">
            <div class="left-part">
                <p class="mb-0 crimson-font">© Copyright 2012 - 2020 | AVADA THEME BY THEMEFUSION | ALL RIGHTS RESERVED |
                    POWERED BY BERNA
                </p>
            </div>
            <div class="right-part">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-x-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-youtube"></i>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
    props: {
        menuItems: {
            type: Array,
            required: true,
        },
    },
}
</script>

<style lang="scss">
@import './style/partials/variables.scss';

footer {
    background-color: $bg-color-dark;

    #footerMenu {
        height: 5rem;
        background-color: $bg-color-dark;

        .footerLogo {
            img {
                padding-left: 1rem;
                height: 1.8rem;
            }
        }

        .footerInfos {
            ul {
                margin-bottom: 0;

                li {
                    list-style: none;
                    font-size: .8rem;
                    margin-right: .5rem;
                    color: $p-text;
                    transition: linear .3s;

                    &:hover {
                        transform: scale(1.1);
                        color: $white;
                    }
                }
            }
        }
    }

    // seconda section
    #copyright {
        height: 5rem;
        background-color: $bg-color-darkest;
        padding: 0 .5rem;

        .left-part {
            color: $p-text;
            font-size: .6rem;

            p {
                transition: linear .3s;

                &:hover {
                    color: $white;
                }
            }
        }

        .right-part {
            color: $p-text;

            i {
                margin-left: .5rem;
                background-color: $bg-color-dark;
                height: 1.5rem;
                width: 1.5rem;
                border-radius: 3px;
                text-align: center;
                line-height: 1.5rem;
                transition: linear .3s;

                &:hover {
                    background-color: white;
                    color: black;
                }
            }
        }
    }
}
</style>
