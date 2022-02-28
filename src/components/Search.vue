<template>
    <form @submit.prevent="ejecutarPeticion">
    <div class="mb-3">
        <label for="inputgif" class="form-label">Categoría</label>
        <input type="text" class="form-control" id="inputgif" aria-describedby="emailHelp"
        v-model="search">
        <div id="emailHelp" class="form-text">Ingresa lo que quieras buscar</div>

    </div>
    <div class="text-center">
        <button type="submit" class="btn btn-default btn-primary w-50">Buscar</button>
    </div>
    </form>
</template>

<script>
export default {
    data: () =>({
        search: "",
    }),
    methods: {
        ejecutarPeticion(){
            this.$emit("accion", this.search)
        }
    }
}
</script>
