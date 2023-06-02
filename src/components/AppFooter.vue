<script>

export default {
    name: 'AppFooter'
}

</script>

<template>
    <footer>
        <div class="nav">
            <div class="col">
                <h3>DC COMICS</h3>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>

                <h3>SHOP</h3>
                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>
            <div class="col">
                <h3>DC</h3>
                <ul>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                    <li></li>
                </ul>
            </div>
            <div class="col"></div>

            <div class="logo-dc">

            </div>
        </div>



        <div class="foot">

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;
@use '../styles/general.scss' as *;

footer {
    color: white;

    .nav {
        @include my-display-flex;
        min-height: 400px;
        background-image: url(../assets/Images/footer-bg.jpg);
        background-color: rgba(0, 0, 0, $alpha: 0.5);



        h3 {
            margin-bottom: 10px;
        }

        ul {
            margin-bottom: 20px;
        }

        li {
            color: grey;
        }
    }
}
</style>