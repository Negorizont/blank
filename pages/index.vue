<template>
  <div class="container">
    <ul class="post-list">
      <li v-for="post of 100" :key="post" class="post">
        <h3 class="post__title">User {{ post }}</h3>
        <p class="post__description">Hello world</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
@import '@/assets/scss/main';
.container {
  max-width: 1200px;
  margin: 0 auto;
}

.post-list {
  width: 100%;
  height: 100vh;
  list-style: none;
  @include flex(column, space-around, center);

  .post {
    padding: 10px;
    border: 1px solid black;
    background-color: red;
    margin-top: 20px;
  }
}
</style>
