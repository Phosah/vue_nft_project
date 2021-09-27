<template>
<div id="alliance-comp">
  <img src="@/assets/allianceComponent/caret.png" @click="showAlliance = !showAlliance">
  <span class="alliance-heading">Alliance</span>
  <div class="allianceComp" v-if="showAlliance">
        <div class="mb-3 d-flex justify-content-start">
            <img class="ms-4" src="@/assets/allianceComponent/group-0.png" />
            <img class="ms-1" src="@/assets/allianceComponent/emojione_handshake-1.png" />
            <img class="ms-1" src="@/assets/allianceComponent/group-1.png" />
        </div>
        <div v-for="alliance in alliances" v-bind:key="alliance.id" class="d-flex alliance align-items-center justify-content-between">
            <div class="mx-4">
                <span>{{ alliance.name }} </span>

                <img :src="alliance.icon">
            </div>

            <span class="value">{{ alliance.value }}</span>
        </div>
    </div>    
</div>
</template>


<script>
    export default {
        data() {
            return {
            showAlliance: true,
            alliances: [
                {
                id: 1,
                name: 'Global Ranking',
                icon: require('@/assets/allianceComponent/vector-1.png'),
                value: '#23'
                },
                {
                id: 2,
                name: 'Cities Controlled',
                icon: require('@/assets/allianceComponent/vector-2.png'),
                value: '21 Cities'
                }
            ]
            }
        },
        methods: {
        }
    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Quattrocento+Sans:wght@700&display=swap');
    #alliance-comp {
    color: #fff;
    }

    .alliance-heading {
    font-size: 0.875rem;
    margin-left: 0.75rem;
    }

    .allianceComp {
    width: 300px;
    min-height: 142px;
    padding: 1.25rem 0;
    background-color: #333333;
    font-family: 'Quattrocento Sans', sans-serif;
    border-radius: 6px;
    }

    .alliance {
    margin-bottom: 0.8125rem;
    }
    
    .value {
        font-size: 0.6875rem;
        margin-right: 21px;
    }
</style>