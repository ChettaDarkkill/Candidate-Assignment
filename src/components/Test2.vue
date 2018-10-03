<template>
    <div>
        <h1>Exercise 2</h1>
        <p>(Y + 24)+(10 × 2) = 99  - Please create new function for finding Y value</p>
            <span>Y = {{ result }}</span>
        <hr />
    </div>
</template>

<script>
export default {
  data () {
    return {
      result: ''
    }
  },
  mounted () {
      this.result = this.Calculate();
  },
  methods : {
      Calculate() {
          var y = 99 - ((10 * 2) + 24);
          return y
      }
  }
}
</script>