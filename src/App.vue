<template>
    <div>
        <v-header></v-header>
        <div class="tab">
            <div class="tab-item">
                <router-link to="/goods">商品</router-link>
            </div>
            <div class="tab-item">
                <router-link to="/ratings">评论</router-link>
            </div>
            <div class="tab-item">
                <router-link to="/sellers">商家</router-link>
            </div>
        </div>
        <router-view></router-view>
    </div>
</template>

<script>
    import Header from './components/header/header.vue';

    export default {
        name: 'app',
        components: {
            'v-header': Header
        }
    };
</script>

<style lang="stylus" rel="stylesheet/stylus">
    .tab
        display: flex
        width: 100%
        height: 40px
        line-height: 40px
        .tab-item
            flex: 1
            text-align: center
</style>
