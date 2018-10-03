<template>
    <div>
        <h1>Exercise 1</h1>
        <p>3, 5, 9, 15, X  - Please create new function for finding X value</p>
            <span>X = {{ result }}</span>
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
     var numbers = [3, 5, 9, 15];
     this.result = this.Calculate(numbers)
  },
  methods : {
      Calculate(numbers) {
            for( var i = 0; i < numbers.length; i++ ) {
                var tmp = 2 * (i + 1)
                if(i == ( numbers.length - 1)) {
                    return numbers[numbers.length - 1] + tmp
                    break;
                }
            }
      }
  }
}
</script>