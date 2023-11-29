<script>
export default {
    name: "appHeader",
    data() {
        return {
            menuList: [
                "CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"
            ]
        }

    }
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-4">
                <img src="/img/dc-logo.png" alt="">

            </div>
            <div class="col-8 d-flex justify-content-between align-items-center">
                <a v-for="item in menuList" href="#">{{ item }}</a>
            </div>
        </div>
    </div>
</template>

<style>
.container {

    padding: 5px;
}

a {
    text-decoration: none;
    color: #222;
    font-weight: bold;
    display: block;
    height: 100
}

img {
    width: 20%;
}
</style>