<script>

export default {
    name: 'AppFooter'
}

</script>

<template>
    <footer>

        <div class="nav">

            <div class="menu-left">
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
                        <li>
                            <a href="#">Terms of use</a>
                        </li>
                        <li>
                            <a href="#">Privacy policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad choises</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">
                                Talent Workshops
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                CPSC Certificates
                            </a>
                        </li>
                        <li>
                            <a href="#">Rating</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h3>Sites</h3>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                </div>
            </div>


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



footer {
    color: white;
    background: url(../assets/Images/dc-logo-bg.png) right center no-repeat, url(../assets/Images/footer-bg.jpg) center center no-repeat, ;
    background-size: 35% auto, cover;
    background-position: 80%, 90%;
    display: flex;
    justify-content: space-around;

    .nav {
        display: flex;


        min-height: 400px;


        align-self: center;

        .menu-left {
            @include center(both);

            .div:last-child {
                display: flex;
            }
        }

        h3 {
            margin-bottom: 10px;
        }

        ul {
            margin-bottom: 20px;
        }

        li {
            color: grey;
            padding: 3px;

            a {
                color: grey;
            }
        }
    }
}
</style>