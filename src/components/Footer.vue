<template>
  <div class="footer mt-auto">
      <footer class="text-center bg-dark text-white py-1 mt-auto bg-gradient">
          <h6>&copy; Aldahir Pulido - {{year}}</h6>
      </footer>
  </div>
</template>
<script>
export default {
    data: () =>({
        year: new Date().getFullYear(),
    }),
}
</script>
<style>
    .footer{
        position: fixed;
        bottom: 0;
        width: 100%;
    }
</style>