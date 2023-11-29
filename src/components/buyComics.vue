<script>
export default {
    name: "buyComics",
    data() {
        return {
            itemList: [
                {
                    icon: "/img/buy-comics-digital-comics.png",
                    name: " DIGITAL COMICS"
                },
                {
                    icon: "/img/buy-comics-merchandise.png",
                    name: " DC MERCHANDISE"
                },
                {
                    icon: "/img/buy-comics-shop-locator.png",
                    name: " SUBSCRIPTION"
                },
                {
                    icon: "/img/buy-comics-subscriptions.png",
                    name: " COMIC SHOP LOCATOR"
                },
                {
                    icon: "/img/buy-dc-power-visa.svg",
                    name: " DC POWER VISA"
                }
            ]
        }
    }
}
</script>
<template>
    <div id="buy-comics">
        <div class="container h-100">
            <div class="row h-100">
                <a href="#" class=" h-100 col d-flex justify-content-between align-items-center">
                    <div v-for="item in itemList" class="item">
                        <img :src="item.icon" :alt="item.name">
                        <span> {{ item.name }}</span>
                    </div>
                </a>
            </div>

        </div>
    </div>
</template>

<style scoped>
#buy-comics {
    height: 15vh;
    background-color: #0282F9;
    position: relative;
    z-index: 1;
}

.item {
    padding: 10px 0;
    color: white;
    cursor: pointer;
}

img {
    width: 2.5rem;
}

a {
    text-decoration: none;
}
</style>