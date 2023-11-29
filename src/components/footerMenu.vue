<script>
export default {
    name: "footerMenu",
    data() {
        return {
            menuList: [
                {
                    title: "DC COMICS",
                    items: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    title: "SHOP",
                    items: [
                        "shop DC",
                        "shop DC Collectibles"
                    ]
                },
                {
                    title: "DC",
                    items: [
                        "Terms Of Use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact us"
                    ]
                },
                {
                    title: "SITES",
                    items: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa"
                    ]
                },
            ]
        }
    }
}
</script>
<template>
    <div id="menu">
        <div class="container h-100">
            <div class="row h-100">
                <div class="col-6 text-white list-wrapper h-100">
                    <ul v-for="list in menuList">
                        <h5>{{ list.title }}</h5>
                        <li v-for="li in list.items">{{ li }}</li>
                    </ul>
                </div>
                <div class="col-6 d-flex justify-content-end">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
#menu {
    height: 40vh;
    background-image: url(/img/footer-bg.jpg);
    padding: .8rem;
    z-index: -1;
}

img {
    position: absolute;
    top: 35%;
    width: 25rem;
    z-index: 0;
}

h5 {
    font-size: 1rem;
}

li {
    list-style: none;
    color: #868989;
    font-size: .7rem;
}

.list-wrapper {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}
</style>