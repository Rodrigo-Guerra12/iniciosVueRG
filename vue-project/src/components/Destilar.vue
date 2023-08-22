<template>
  <div class="card">
    <div class="card2">
      <img :src="image" alt="Banda de Música" />
      <h1>{{ disco }}</h1>

      <div>
        <button>Buy Now!</button> <br />
        <a :href="info">Info</a>
      </div>
    </div>
    <div class="descript">
      <p>{{infoCD}}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {},
  data() {
    return {
      image:
        "https://www.zonadeobras.com/wp-content/uploads/2018/08/vela-cuadrada.jpg",
      disco: "Destilar",
      info: "https://www.palaciodelamusica.com.uy/catalogo/la-vela-puerca-destilar-cd_190758606323_190758606323",
      infoCD: 'La banda uruguaya presenta Destilar, su séptimo álbum de estudio en veintidós años de vida. Inspirado en las sierras cordobesas de Argentina, el disco exprime infinidad de sentimientos con esa sutileza artística marca de la casa. La Vela Puerca no defrauda nunca.'
    };
  },
};
</script>

<style scoped>
h1 {
  font-size: 20px;
}

.card {
  display: flex;
  justify-content: space-between;
  /* border: 1px solid #ccc; */
  padding: 15px;
  margin: 10px;
  text-align: center;
  width: 25vw;
  height: 15vw;
}

a {
  font-size: 12px;
  font-family: poppins;
  color: blue;
  text-decoration: underline;
}
.descript {
  font-size: 10px;
}

img {
  max-width: 80%;
  height: auto;
}

button{
    width: 4rem;
    font-size: 10px;
  }

button:hover {
  cursor: pointer;
  box-shadow: inset 1px 2px 20px 0 blue;
}
</style>
