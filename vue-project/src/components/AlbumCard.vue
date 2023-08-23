<script>
export default {
  props: {
    album: Object
  }
}
</script>

<template>
  <h2>Album card</h2>
  <h2>{{ album.name || 'No props passed yet' }}</h2>
</template>