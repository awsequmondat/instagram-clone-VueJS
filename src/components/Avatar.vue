<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size" />
  </figure>
</template>

<script>
export default {
  name: 'Avatar',
  props: {
    src: {
      type: String,
      default:
        'https://instagram.fada2-1.fna.fbcdn.net/v/t51.2885-19/s150x150/82051726_182131399700831_2537802295811244032_n.jpg?_nc_ht=instagram.fada2-1.fna.fbcdn.net&_nc_ohc=pSif1OA1DrAAX-ll4np&oh=46c883c56a69e560083421dfcd86fc5a&oe=5F81D106'
    },
    alt: {
      type: String
    },
    size: {
      type: Number
    }
  }
}
</script>

<style scoped>
.avatar {
  display: inline-flex;
  padding: 2px;
  border-radius: 999px;
  background: linear-gradient(
    219deg,
    rgba(184, 63, 140, 1) 0%,
    rgba(237, 158, 90, 1) 100%
  );

  img {
    border-radius: inherit;
    border: 2px solid white;
  }
}
</style>
