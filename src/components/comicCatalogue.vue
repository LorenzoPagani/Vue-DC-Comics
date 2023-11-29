<script>
export default {
    name: "comicCatalogue",
    props: ["cards"]
}
</script>
<template>
    <div id="catalogue">
        <img class="jumbo" src="/img/jumbotron.jpg" alt="">
        <div class="container">
            <button type="button" class="btn btn-primary">CURRENT SERIES</button>
            <div class="row">
                <div class="col-12 d-flex justify-content-between flex-wrap">
                    <div v-for="card in cards" class="my-card text-white">
                        <img class="cover" :src="card.thumb" alt="">
                        <p class="mb-0">{{ card.series }}</p>
                        <p class="mt-0">{{ card.price }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
#catalogue {
    background-color: #1C1C1C;
}

.container {
    position: relative;
}

.btn-primary {
    position: absolute;
    top: -7%;
    border-radius: 0;
}

.jumbo {
    width: 100%;
    height: 30vh;
    object-fit: cover;
    object-position: top;
    margin-bottom: 2rem;
}

.my-card {
    width: calc(100% / 6);
    padding: 0 1rem;
    margin: 2rem 0;
    cursor: pointer;
}

.cover {
    width: 100%;
    aspect-ratio: 2 / 3;
}
</style>