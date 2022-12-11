<template>
  <div class="page-title">
    <h1>
        {{page_title}}
    </h1>
  </div>
</template>

<script>
export default {
    props: ['page_title']

}
</script>

<style lang="scss">
.page-title {
    h1 {
        font-size: 3.222em;
    }
}
</style>