<template>
  <div class="card">
    <div class="card2">
      <img :src="image" alt="Banda de Música">
      <h1>{{disco}}</h1>
            
      <div>
        <button>Buy Now!</button> <br>
        <a :href="info">Info</a>
      </div>
    </div>
    <div class="descript">
      <p>{{ infoCD }}</p>
    </div>
  </div>
  
  <div :albums="albums[0]">
    <h2>{{ almbums }}</h2> 
  </div>

</template>
  
  <script>
  export default {
    props: {
      albums:Object    },
    data() {
      return {
        image: 'https://i.discogs.com/C63BrcGnLWn41Nai5npHGJs5tZLluOnsMRLclBQ-tE0/rs:fit/g:sm/q:40/h:300/w:300/czM6Ly9kaXNjb2dz/LWRhdGFiYXNlLWlt/YWdlcy9SLTY3NTYx/MTgtMTQyNTk2NjMx/Ni0xMzkyLmpwZWc.jpeg',
        disco: 'Deskarado',
        info: 'https://www.palaciodelamusica.com.uy/catalogo/la-vela-puerca-deskarado-cd_OBL1502-2_OBL1502-2',
        infoCD: 'Deskarado es el primer álbum de la banda uruguaya de rock La Vela Puerca. Fue grabado a fines de 1997 y publicado en marzo de 1998 por el sello independiente Obligado Records, y contó con la producción del músico uruguayo Claudio Taddei. El álbum tuvo una buena difusión y fue un gran éxito de ventas llegando a conseguir un disco de oro y uno de platino.'
      };
    }
  };
  </script>
  
  <style scoped>
  h1 {
    font-size: 18px;
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
  