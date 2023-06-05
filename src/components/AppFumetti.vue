<script>

export default {
    name: 'AppFumetti',
    props: {
        details: Object
    }
}

</script>

<template>
    <div class="card">
        <img :src="details.thumb" alt="">
        <h4>{{ details.series }}</h4>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

.card {
    display: flex;
    padding: 20px;
    flex-direction: column;
    height: 202px;
    width: calc(100% / 6);
    margin-bottom: 25px;

    img {
        width: 100%;
        height: 162px;
        object-fit: cover;
    }

    h4 {
        margin: 15px 0;
        color: white;
    }
}
</style>