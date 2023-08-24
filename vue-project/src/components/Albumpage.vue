<script>
import AlbumCard from "./AlbumCard.vue";

export default {
  components: {
    AlbumCard,
  },
  data() {
    return {
      albums: [
        {
          name: "Deskarado",
          imgURL:
            "https://i.discogs.com/C63BrcGnLWn41Nai5npHGJs5tZLluOnsMRLclBQ-tE0/rs:fit/g:sm/q:40/h:300/w:300/czM6Ly9kaXNjb2dz/LWRhdGFiYXNlLWlt/YWdlcy9SLTY3NTYx/MTgtMTQyNTk2NjMx/Ni0xMzkyLmpwZWc.jpeg",
          description:
            "Deskarado es el primer álbum de la banda uruguaya de rock La Vela Puerca. Fue grabado a fines de 1997 y publicado en marzo de 1998 por el sello independiente Obligado Records, y contó con la producción del músico uruguayo Claudio Taddei. El álbum tuvo una buena difusión y fue un gran éxito de ventas llegando a conseguir un disco de oro y uno de platino.",
        },
        {
          name: "Acontraluz",
          imgURL:
            "https://upload.wikimedia.org/wikipedia/en/3/30/Velapuercatapa.jpg",
          description:
            "A contraluz es el tercer álbum de La Vela Puerca, su tapa es de color amarillo, editado en el 2004. Fue producido por Gustavo Santaolalla2​ y grabado en Del Cielito Records, Buenos Aires. Entre los invitados figuran: Toto Méndez y sus compadres, el violista Gian Di Piramo, y el violinista Javier Casalla.",
        },
        {
          name: "De Bichos y Flores",
          imgURL:
            "https://http2.mlstatic.com/D_NQ_NP_638454-MLA40025109336_122019-O.webp",
          description:
            "De bichos y flores es el segundo disco de La Vela Puerca, editado en 2001. Algunos de sus temas más exitosos son El Viejo, Por Dentro, El Profeta, Burbujas, y Por la Ciudad. El disco fue grabado en los estudios Panda y La Casa de Los Ángeles por Ricardo Troilo y Aníbal Kerpel respectivamente. La producción artística estuvo a cargo de Gustavo Santaolalla. ",
        },
        {
          name: "El Impulso",
          imgURL: "https://www.cmtv.com.ar/tapas-cd/velaimpulso.webp",
          description:
            "El impulso es el cuarto disco de la banda uruguaya de rock/ska La Vela Puerca. Fue lanzado en abril de 2007. El álbum fue grabado y masterizado por Julio Berta en el período noviembre/diciembre de 2006. La grabación fue realizada en tres estudios diferentes: Panda Studios en Buenos Aires, IFU en Montevideo, y Casa Blanca en Atlántida. La masterización fue ideada durante febrero de 2007.",
        },
      ],
    };
  },
};
</script>

<template>
  <h1>La Vela Puerca</h1>
  <div class="container">
    <AlbumCard :album="albums[0]" />
    <AlbumCard :album="albums[1]" />
    <AlbumCard :album="albums[2]" />
    <AlbumCard :album="albums[3]" />
  </div>
</template>

<style>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

#app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;
}
</style>
