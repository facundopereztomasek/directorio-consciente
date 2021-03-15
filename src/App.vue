<template>
  <div class="main">
    <h1>Directorio Consciente</h1>
    <hr />
    <div class="content-item-title">
      <div class="image-wrapper">
        <img
          class="image"
          :src="require('@/assets/vejolk.jpg')"
          alt="Vjolk Distribuidora"
        />
      </div>
      <div>
        <h2 class="title">Vejølk</h2>
        <h3 class="subtitle">
          Distribuidora de Alimentos y articulos exclusivamente Veganos
        </h3>
      </div>
    </div>
    <div class="content-item-data">
      <p class="label">Teléfono</p>
      <p class="data">
        <a
          ref="noopener noreferrer"
          target="_blank"
          href="tel:+54 9 11 5095 2174"
          >+54 9 11 5095 2174</a
        >
      </p>
      <p class="label">Instagram</p>
      <p class="data">
        <a
          ref="noopener noreferrer"
          target="_blank"
          href="https://www.instagram.com/vejolk"
          >@vejolk</a
        >
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style lang="scss" scoped>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2,
h3,
p {
  margin: 0;
}

.main {
  font-family: Avenir, Helvetica, Arial, sans-serif;

  .content-item-title {
    margin-bottom: 20px;
  }

  .content-item-title,
  .content-item-data {
    display: grid;
    grid-template-columns: 100px 1fr;
    grid-gap: 10px 20px;
    align-items: center;

    & > * {
      &:nth-child(even) {
        justify-self: start;
      }
      &:nth-child(odd) {
        justify-self: end;
      }
    }
  }
  .image-wrapper {
    overflow: hidden;
    border-radius: 100%;
    .image {
      width: 60px;
      height: 60px;
      vertical-align: bottom;
    }
  }
}
</style>
