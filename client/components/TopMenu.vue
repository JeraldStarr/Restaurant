<template>
  <div class="top-menu text-center">
    <div class="d-flex justify-content-center align-items-center">
      <nuxt-link to="/">Starters</nuxt-link>
      <span class="dot"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/lunch">Lunch</nuxt-link>
      <span class="dot"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/desserts">Desserts</nuxt-link>
      <span class="dot"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/yourorder">Your Order <i class="bi bi-bag"></i> (0)</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .top-menu {
    margin: 42px;
    .goldenline {
      border-bottom: 1px solid goldenrod;
      &::after {
        display: block;
        content: "";
        height: 1px;
        width: 83%;
        background-color: goldenrod;
        position: relative;
        top: 8px;
        margin: 0 auto;
      }
    }
    a {
      color: #495057;
      text-transform: uppercase;
      font-size: 22px;
      font-weight: 300;
      text-decoration: none;
      border-bottom: 1px solid transparent;
      &.nuxt-link-exact-active {
        @extend .goldenline;
      }
      &:hover {
        border-bottom: 1px solid goldenrod;
      }
    }
    .dot {
      display: inline-block;
      color: goldenrod;
      font-size: 8px;
      margin-right: 20px;
      margin-left: 20px;
    }
  }
</style>
