<template>
    <div>
        <p v-for="(item, index) in this.$store.state.news" :key="index">
            <a v-bind:href="item.url">
                {{ item.title }}
            </a>
            <small>
                {{ item.time_ago }} by 
                <router-link v-bind:to="'/user/' + item.user">{{ item.user }}</router-link>
                <!-- <router-link v-bind:to="`/user/${item.user}`">{{ item.user }}</router-link> -->
            </small>
        </p>
    </div>
</template>

<script>
export default {
    created(){
        this.$store.dispatch('FETCH_NEWS');
    }
}
</script>

<style>

</style>