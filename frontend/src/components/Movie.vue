<template>
  <div>
    <div>
      {{ movie.original_title }}
      {{ movie.released_date }}
    </div>
    <img :src="'https://image.tmdb.org/t/p/w200' + movie.poster_path" />
  </div>
</template>

<script>
export default {
  name: "Movie",
  props: {
    movie: Object,
  },
};
</script>
