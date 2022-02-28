<template>
<div class="container mt-3">
  <div class="card" style="width: 100%;">
    <div class="card-body">
      <h5 class="card-title fs-2">Gif Router</h5>
      <h6 class="card-subtitle mb-2 text-muted fs-4">Creado por: Aldahir Pulido</h6>
      <p class="card-text fs-5" style="text-align: justify">Aplicación creada en el curso de Vue 3 en Udemy, integrando Bootstrap, rutas, etc.
        Esta aplicación utiliza la API gratuita de <a href="https://developers.giphy.com/" target="_blank" class="text-decoration-none">Giphy</a> para mostrar elementos de tipo gif y sticker.
        Dichos elementos utilizan la librería <a href="https://www.npmjs.com/package/vue-axios" target="_blank" class="text-decoration-none">Axios</a> para realizar las peticiones que ayudan a mostrar la información 
        (en este caso gifs/stickers) deaseados.
      </p>
      <p class="card-text fs-5" style="text-align: justify">Debajo se encuentran enlaces directos a la documentación oficial de Boostrap y VueJS en su tercera versión.</p>
      <div class="text-center">
        <a href="https://getbootstrap.com/" target="_blank" class="card-link"><img src="https://brandlogos.net/wp-content/uploads/2021/09/bootstrap-logo.png" width="15%" alt="Bootstrap-Logo"></a>        
        <a href="https://vuejs.org/" target="_blank" class="card-link"><img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg" width="10%" alt="Bootstrap-Logo"></a>
      </div>
    </div>
  </div>
</div>
</template>

<style scoped>
  img{
    transition: transform 500ms;
  }
  img:hover{
    transform: scale(0.5);
  }
</style>

