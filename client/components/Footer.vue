<template>
    <footer class="footer">
        <Logo/>
      <div class="footer__menu d-flex justify-content-center align-items-center">
        <span>Copyright &copy; 2021 d'Orellia</span>
        <span class="dot"><i class="bi bi-circle-fill"></i></span>
        <nuxt-link to="/">Privacy Policy</nuxt-link>
        <span class="dot"><i class="bi bi-circle-fill"></i></span>
        <nuxt-link to="/">Terms of Use</nuxt-link>
        <span class="dot"><i class="bi bi-circle-fill"></i></span>
        <nuxt-link to="/">Contact</nuxt-link>
      </div>

    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.footer {
  margin: 72px auto;
    .logo {
        img {
            width: 150px;
        }
    }
  &__menu {
    margin-top: 22px;
  }
  a {
    color: #495057;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: 300;
    text-decoration: none;
    border-bottom: 1px solid transparent;
    &:hover {
      color: goldenrod;
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
