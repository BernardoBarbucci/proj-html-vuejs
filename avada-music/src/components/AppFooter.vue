<template>
    <footer class="container-fluid">
        <section id="footerMenu" class="col-12 d-flex align-items-center justify-content-between">
            <div class="footerLogo">
                <img src="./style/img/logo_footer.png" alt="logo footer">
            </div>
            <div class="footerInfos">

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
    }
}
</style>