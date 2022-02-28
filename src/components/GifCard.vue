<template>
<div class="card" style="width: 18rem;">
    <img :src="data.images.downsized.url" class="card-img-top" alt="Gif">
    <div class="card-body">
        <h5 class="card-title text-center" v-if="data.username">Autor: {{ data.username }}</h5>
        <h5 class="card-title text-center" v-else>Autor: Desconocido</h5>
        <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
    </div>
</div>
</template>
<script>
export default {
    props: {
        data: Object,
    },
};
</script>
