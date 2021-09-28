<template>
    <div class="cont">
        <nav>
            <navbar/>
        </nav>

        <b-row class="Collec">
            <h2 class="m-5">Collectibles</h2>
        </b-row>

        <b-row align-h="between">
            <b-col><butttonGroup/></b-col>
            <b-col class=" end-this v-al mt-3">
                <span class=" ending army-heading">Recently Added</span>
                <div>
                    <img src="../assets/armyComponent/caret.png" @click="showArmyMood" ref="caret" class="caret">
                </div>
                
            </b-col>
        </b-row>

        <b-row class="m-3">
            <card-grid/>
        </b-row>

        <b-row>
            <b-col md="3" v-for="(item, index) in pool" :key="index">
                <nft-card/>
            </b-col>
        </b-row>
    </div>
</template>


<script>
import Navbar from '../components/Navbar.vue'
import NftCard from '../components/nftCard.vue'
import cardGrid from '../components/cardGrid.vue'
import butttonGroup from '../components/buttonGroup.vue'

export default {
    name: "nftCard",
    data(){
        return{
            showArmy: false,
        }
    },
    components:{
        NftCard,
        Navbar,
        butttonGroup,
        cardGrid
    },
    methods:{
        showArmyMood(){
        this.showArmy = !this.showArmy
        this.$refs.caret.classList.toggle("rotate")
    }
    }

}

</script>

<style scoped>

.cont{
    background-color: rgba(34, 34, 34, 1);
}

.v-al{
    vertical-align: middle;
}

.end-this{
    display: flex;
    justify-content: end;
    padding-right: 4rem;
}

.ending{
    text-align: end;
    padding-right: 0.5rem;
}

.Collec{
    color: white;
}

span{
    color: white;
}

.caret{
    transform: rotate(0deg);
    cursor: pointer;
}

.caret.rotate{
    transform: rotate(180deg);
}

</style>