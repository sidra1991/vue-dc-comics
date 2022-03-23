<template>
  <div class="black" >
      <div class="bl-left">
        <p>content goes here</p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'BlackLine'
}
</script>

<style scoped lang="scss">
  .black{
    height: 100px;
    color: white;

  }

  .bl-left {
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

</style>
