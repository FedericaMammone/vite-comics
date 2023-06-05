<script>

export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: false
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: true
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                }
            ]
        }
    }


}

</script>

<template>
    <header>
        <div class="logo">
            <img src="../assets/Images/dc-logo.png" alt="">
        </div>

        <div class="menu">
            <nav>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.src">
                            <strong>
                                {{ link.text }}
                            </strong>
                        </a>
                    </li>

                </ul>
            </nav>
        </div>

    </header>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;
@use '../styles/general.scss' as *;

header {
    @include my-display-flex;

    height: 100px;
    background-color: white;


    .logo {
        width: 70px;
        height: 70px;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }

    nav {

        ul {
            display: flex;


            li {
                list-style-type: none;
                padding: 10px;
                font-size: 10px;

                &:hover {
                    cursor: pointer;
                    color: $primary;
                }
            }
        }

    }
}
</style>