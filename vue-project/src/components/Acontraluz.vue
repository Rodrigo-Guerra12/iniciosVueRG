<template>
  <div class="card">
      <div class="card2">
          <img :src="image" alt="Banda de Música">
          <h1>{{disco}}</h1>
          
          <div>
              <button >Buy Now!</button> <br>
              <a :href="info">Info</a>
          </div>
      </div>
      <div class="descript">
        <p>
        {{ infoCD }}
      </p>
          
          
        

      </div>
  </div>
</template>

<script>
export default {
  props: {
    
  },
  data() {
    return {
      image: 'https://1.bp.blogspot.com/-Qad6s579upA/XeoydwiXk1I/AAAAAAAAHpI/9V0vrScwdM8CZdHWlXJiSaniYnRRm8qLQCEwYBhgL/s1600/41CqTnqn5vL._SX355_.jpg',
      disco: 'A Contraluz',
      info: 'https://www.palaciodelamusica.com.uy/catalogo/la-vela-puerca-a-contraluz-cd_9822076_9822076',
      infoCD: ' A contraluz es el tercer álbum de La Vela Puerca, su tapa es de color amarillo, editado en el 2004. Fue producido por Gustavo Santaolalla2​ y grabado en Del Cielito Records, Buenos Aires. Entre los invitados figuran: Toto Méndez y sus compadres, el violista Gian Di Piramo, y el violinista Javier Casalla.'
      
    };
  }
};
</script>

<style scoped>
h1 {
  font-size: 20px;
}

a {
  font-size: 12px;
  font-family: poppins;
  color: blue;
  text-decoration: underline;
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
