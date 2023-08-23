<script >
import AlbumCard from './AlbumCard.vue';

export default {
  components: {
    AlbumCard
  },
  data() {
    return {
      albums: [
        {
          name: 'Deskarado',
          imgURL: 'https://i.discogs.com/C63BrcGnLWn41Nai5npHGJs5tZLluOnsMRLclBQ-tE0/rs:fit/g:sm/q:40/h:300/w:300/czM6Ly9kaXNjb2dz/LWRhdGFiYXNlLWlt/YWdlcy9SLTY3NTYx/MTgtMTQyNTk2NjMx/Ni0xMzkyLmpwZWc.jpeg',
          description: 'HolaHolaHolaHolaHolaHolaHolaHolaHolaHolaHola'
        }
      ]
    }
  }
}
</script>

<template>
  <h1>Album Page</h1>
  <AlbumCard :album="albums[0]" />
</template>



<style>
#app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;

}

.conrating {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.Cards {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 25px;
  max-width: 100%;
}

.sombra {
  border: solid 0.1px rgb(61, 59, 59);
  margin: 10px;
  height: auto;
}

.sombra:hover {
  cursor: pointer;
  box-shadow: inset 1px 2px 20px 0 blue;
}
</style>
