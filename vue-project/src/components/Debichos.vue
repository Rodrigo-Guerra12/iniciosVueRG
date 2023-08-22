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
        image: 'https://administrador.m24.com.uy/wp-content/uploads/2021/08/De-Bichos-y-Flores.jpg',
        disco: 'De Bichos Y Flores',
        info: 'https://www.palaciodelamusica.com.uy/catalogo/la-vela-puerca-de-bichos-y-flores-cd_016070-2_016070-2',
        infoCD: 'De bichos y flores es el segundo disco de La Vela Puerca, editado en 2001. Algunos de sus temas más exitosos son El Viejo, Por Dentro, El Profeta, Burbujas, y Por la Ciudad. El disco fue grabado en los estudios Panda y La Casa de Los Ángeles por Ricardo Troilo y Aníbal Kerpel respectivamente.'
        
        
      };
    }
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
  box-shadow: inset 1px 2px 20px 0 blue; }
  </style>
  