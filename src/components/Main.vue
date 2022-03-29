<template>
    <div>
        <MainJumbotron/>
        <MainCards/>
    </div>
</template>

<script>
import MainJumbotron from './MainJumbotron.vue';
import MainCards from './MainCards.vue'

export default {
    components:{
        MainJumbotron,
        MainCards
    },
    name: "IndexMain"
}
</script>

<style lang="scss" scoped>

</style>