<template>
  <div class="page-title">
    <div class="d-flex justify-content-center align-items-center">
      <div class="left-ornament"></div>
      <h1>
        {{page_title}}
      </h1>
      <div class="right-ornament"></div>
    </div>
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
      padding: 0 32px;
    }
  .left-ornament {
    position: relative;
    width: 100%;
    height: 1px;
    background-color: goldenrod;
    &::before {
      display: block;
      content: "";
      height: 1px;
      width: 70px;
      background-color: goldenrod;
      position: absolute;
      bottom: 8px;
      right: 8px;
    }
    &::after {
      display: block;
      content: "";
      height: 1px;
      width: 70px;
      background-color: goldenrod;
      position: absolute;
      top: 8px;
      right: -8px;
    }
  }
  .right-ornament {
    position: relative;
    width: 100%;
    height: 1px;
    background-color: goldenrod;
    &::before {
      display: block;
      content: "";
      height: 1px;
      width: 70px;
      background-color: goldenrod;
      position: absolute;
      bottom: 8px;
      left: 8px;
    }
    &::after {
      display: block;
      content: "";
      height: 1px;
      width: 70px;
      background-color: goldenrod;
      position: absolute;
      top: 8px;
      left: -8px;
    }
  }
}
</style>
