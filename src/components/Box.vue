<template>
  <div class="box-project mt-4 mb-4 me-4" :style='{backgroundImage: "url(" + img + ")", }'>
    <div class="bg-trasparenza">
      <div class="name-project">
        {{titolo}}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Box",
  props: ['titolo', 'img'],
}
</script>

<style lang ="scss" scoped>

  .box-project {
    background-size: contain;
    background-repeat: no-repeat;
    width: 400px;
    height: 400px;
    border-radius: 5px;
    .bg-trasparenza {
      height: 100%;
      width: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      .name-project {
        color: #ffffff;
        font-size: 1.8em;
        padding: 260px 10px 0 10px;
        font-weight: bold;
      }
    }
  }
</style>