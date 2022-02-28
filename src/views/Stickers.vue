<template>
    <div class="container mt-3 border ">
        <h1 class="text-center">Stickers</h1>
        <search @accion="getStickers"/>
        <hr />
        <loading v-if="load" />
        <div class="row">
            <div class="col-12 col-lg-3 d-flex" v-for="sticker in stickers" :key="sticker.id">
                <sticker-card :data="sticker" class="m-auto mb-3 w-100%" />
            </div>
        </div>
    </div>
</template>

<script>
import Loading from '../components/Loading.vue';
import StickerCard from '../components/StickerCard.vue';
import Search from '../components/Search.vue';
export default {
    components: { Search, Loading, StickerCard, },
    data: () =>({
        stickers: {},
        load: false,
    }),
    created(){
        this.getStickers();
    },
    methods: {
        async getStickers(search = ""){

            this.load = true;

            const key = "go3QQQUl7nXiNwmyg2G8kJZ0rpT0g46o"
            const {data} = await this.axios.get(
                `https://api.giphy.com/v1/stickers/search?q=${search}&api_key=${key}`
                );
            this.stickers = data.data;
            this.load = false;
        }
    }
}
</script>
