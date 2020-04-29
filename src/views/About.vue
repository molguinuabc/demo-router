<template>
  <div class="container">
    <h1>Esta es la página de About</h1>
    <h2>Este es el contenido de $route.params: {{ $route.params }}</h2>
    <br />
    <button class="btn btn-primary m-2" @click="regresaConPush">
      Regresa a casa con push
    </button>
    <button class="btn btn-info m-2" @click="regresaConReplace">
      Regresa a casa con replace
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    regresaConPush() {
      this.$router.push("/");
    },
    regresaConReplace() {
      this.$router.replace({ name: "casa" });
    }
  }
};
</script>
