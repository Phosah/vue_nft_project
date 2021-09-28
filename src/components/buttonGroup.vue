<template>
    <div class="mx-4 my-3">
        <b-button-group size="">
            <b-button class="blackMe">All</b-button>
            <b-button class="blackMe">Artifacts</b-button>
            <b-button class="blackMe">Territories</b-button>
            <b-button class="blackMe">Armies</b-button>
        </b-button-group>
    </div>
</template>

<script>
export default {
    name: "butttonGroup",
    data(){
        return{

        }
    }
}

</script>

<style scoped>

.blackMe {
    background-color: #333232 !important;
}

</style>