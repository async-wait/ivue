<template>
  <div>
    <header>这是children1</header>
    <Children2
      v-bind="$attrs"
    ></Children2>
  </div>
</template>

<script>
import Children2 from './children2';
export default {
  components: {
    Children2
  },
  props: {
    foo: String
  },
  inheritAttrs: false,
  created() {
    console.log(this.$attrs);
  },
  data() {
    return {

    }
  },
  methods: {

  }
}
</script>

<style lang="less" scoped>

</style>
