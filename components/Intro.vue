<template>
  <section id="intro" class="level">
    <div class="level-left" v-editable="blok">
      <p class="blurb">{{ blok.blurb }}</p>
    </div>
    <div class="level-right">

    </div>
  </section>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #intro{
    padding: 30px;
    border-bottom: 1px solid #f4efe9;
  }
  .level-left{
    max-width: 60vw;
    text-align: left;
  }
  .level{
  margin-bottom: 0 !important;
}
</style>
