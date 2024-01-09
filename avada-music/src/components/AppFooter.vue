<template>
    <footer class="container-fluid">
        <section id="footerMenu" class="col-12 d-flex align-items-center justify-content-between">
            <div class="footerLogo">
                <img src="./style/img/logo_footer.png" alt="logo footer">
            </div>
            <div class="footerInfos">
                <ul class="d-flex flex-row">
                    <li>Home</li>
                    <li>Meet the Band</li>
                    <li>Live Dates</li>
                    <li>Latest News</li>
                    <li>Albums</li>
                    <li>Fans</li>
                </ul>
            </div>
        </section>
        <section id="copyright" class="col-12 d-flex align-items-center justify-content-between">
            <div class="left-part">
                <p></p>
            </div>
            <div class="right-part">
                <!-- inserire icone da fontawesome dei 4 social (fb, X, insta, youtube) -->
            </div>
        </section>
    </footer>
</template>
<script>
export default {
    name: 'AppFooter',
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
    }
}
</style>

