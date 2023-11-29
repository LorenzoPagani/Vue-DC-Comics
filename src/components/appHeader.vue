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
    <header>
        <div class="container h-100">
            <div class="row align-items-center h-100 ">
                <div class="col-5">
                    <img src="/img/dc-logo.png" alt="">
                </div>
                <div class="col-7 d-flex justify-content-between align-items-center">
                    <a v-for="item in menuList" href="#">{{ item }}</a>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
header {
    height: 15vh;
}

.container {
    padding: 5px;
}

a {
    text-decoration: none;
    color: #222;
    font-weight: bold;
    font-size: .8em;
}

img {
    width: 4rem;
}
</style>