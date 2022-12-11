<template>
    <div class="container">
        <div class="p-3">
            <Logo/>
            <TopMenu/>
            <Nuxt/>
            <Footer/>
        </div>
    </div>
</template>

<script>
import TopMenu from '../components/TopMenu.vue'

export default {
  components: { TopMenu },
    layout: 'homepage',
}
</script>