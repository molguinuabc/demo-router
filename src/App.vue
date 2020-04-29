<template>
  <div id="app">
    <div class="row d-flex vh-100">
      <div class="col col-2  bg-light font-weight-bold text-center">
        <div class="pt-4">
          <div class="mb-4">
            <router-link to="/">Principal</router-link>
          </div>
          <div class="mb-4">
            <router-link :to="{ name: 'About' }">Acerca</router-link>
          </div>
        </div>
      </div>
      <div class="col pl-5 pt-3 principal">
        <router-view />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      datos: {
        id: 1,
        nombre: "John Doe"
      }
    };
  }
};
</script>
<style>
.principal {
  background-color: beige;
}
</style>
