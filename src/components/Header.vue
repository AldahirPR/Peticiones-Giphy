<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark bg-gradient">
  <div class="container-fluid">
    <!-- <a class="navbar-brand" href="/about">Gif Routes</a> -->
    <router-link class="navbar-brand" to="/">Gif Router</router-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <!-- <a class="nav-link active" aria-current="page" href="#">Home</a> -->
            <router-link class="nav-link active" aria-current="page" to="/">Home</router-link>
        </li>
        <li class="nav-item">
          <!-- <a class="nav-link" href="#">Features</a> -->
            <router-link class="nav-link" aria-current="page" to="/Gifs">Gifs</router-link>
        </li>
        <li class="nav-item">
          <!-- <a class="nav-link" href="#">Features</a> -->
            <router-link class="nav-link" aria-current="page" to="/Stickers">Stickers</router-link>
        </li>
        <li class="nav-item">
          <!-- <a class="nav-link" href="#">Features</a> -->
            <router-link class="nav-link" aria-current="page" to="/About">About</router-link>
        </li> 
      </ul>
    </div>
  </div>
</nav>
</template>

<script>
export default {

}
</script>
