<template>
    <div>
        <div class="my-5">
            <div class="d-flex justify-content-between my-2">
                <div @click="showMore"><img src="../assets/up-arrow.png" alt="Arrow icon"></div>
                <div class="collectibles-title">Collectibles</div>
                <div><img src="../assets/dots.png" alt="Dot icon"></div>
            </div>

            <div v-for="collectible in collectiblesOne" :key="collectible.name" class="collectibles-block d-flex justify-content-center align-items-center flex-wrap rounded-3">

                <div class="collectibles-item-box mb-3 mx-2">
                    <div class=""><img class="collectibles-item__photo" :src="collectible.image" alt="Power Stone"></div>
                    <p class="mb-1 text-center">{{ collectible.name }}</p>
                    <div class="d-flex justify-content-center">
                        <div class="collectibles-item__icon-box d-flex align-items-center me-2 px-2 rounded-pill">
                            <div class="me-1"><img class="collectibles-item__icon" src="../assets/fire.png" alt="Fire photo"></div>
                            <div class="collectibles-item__text">{{ collectible.firePoints }}</div>
                        </div>
                        <div class="d-flex collectibles-item__icon-box align-items-center px-2 rounded-pill">
                            <div class="me-1"><img class="collectibles-item__icon" src="../assets/lightening.png" alt="Fire photo"></div>
                            <div class="collectibles-item__text">{{ collectible.lightPoints }}</div>
                        </div>
                    </div>
                </div>
                <!--  -->

                 <div class="collectibles-item-box mb-3 mx-2">
                    <div class=""><img class="collectibles-item__photo" :src="collectible.image" alt="Power Stone"></div>
                    <p class="mb-1 text-center">{{ collectible.name }}</p>
                    <div class="d-flex justify-content-center">
                        <div class="collectibles-item__icon-box d-flex align-items-center me-2 px-2 rounded-pill">
                            <div class="me-1"><img class="collectibles-item__icon" src="../assets/fire.png" alt="Fire photo"></div>
                            <div class="collectibles-item__text">{{ collectible.firePoints }}</div>
                        </div>
                        <div class="d-flex collectibles-item__icon-box align-items-center px-2 rounded-pill">
                            <div class="me-1"><img class="collectibles-item__icon" src="../assets/lightening.png" alt="Fire photo"></div>
                            <div class="collectibles-item__text">{{ collectible.lightPoints }}</div>
                        </div>
                    </div>
                </div>
                <!--  -->
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            showCollectibles: true,
            collectiblesOne: [
                {
                    name: "Power Stone",
                    image: require("../assets/power-stone.png"),
                    lightPoints: 24,
                    firePoints: 24
                },
                {
                    name: "Edga's Ring",
                    image: require("../assets/edga-ring.png"),
                    lightPoints: 22,
                    firePoints: 56
                }

            ],
            collectiblesTwo: [
                {
                    name: "Moon Tear",
                    image: require("../assets/moon-tear.png"),
                    lightPoints: 16,
                    firePoints: 67
                },
                {
                    name: "Power Portion",
                    image: require("../assets/power-portion.png"),
                    lightPoints: 18,
                    firePoints: 39
                },

            ],
        }
    },
    methods: {
        showMore() {
            this.showCollectibles = false;

        }
    }
    
}
</script>

<style scoped>
.collectibles-block {
    background-color: #333333;
    width: 300px;
    padding: 20px 20px 10px 20px;
}
.collectibles-title {
    font-size: 20px;
}
.collectibles-item-box {
    width: 43.5%;
}
.collectibles-item__icon {
    width: 10px;
}
.collectibles-item__icon-box {
    background-color: #404040;
}
.collectibles-item__text {
    font-size: 10px;
}
.collectibles-item__photo {
    width: 100%;
}
</style>