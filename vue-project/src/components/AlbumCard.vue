<script>
export default {
  props: {
    album: Object,
  },
  methods: {
    alert1() {
      window.alert("Compraste el CD ");
    },
  },
};
</script>

<template>
  <div class="contenido">
    <div class="card">
      <h3>{{ album.name }}</h3>
      <img :src="album.imgURL" /> <br />
      <button @click="alert1">Buy Now!</button>
    </div>

    <p>{{ album.description }}</p>
   
    
  </div>
</template>

<style scoped>
.contenido {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  border: solid black 1px;
  margin: 10px;
  padding: 10px;
  width: 20rem;
  background-color: rgb(168, 166, 166);
}

p {
  font-size: 10px;
}
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 10px;
}

img {
  width: 7rem;
  margin: 5px;
}

button {
  margin: 10px;
  border-color: blue;
  border-radius: 4px;
}
</style>
