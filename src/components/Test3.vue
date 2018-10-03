<template>
    <div>
        <h1>Exercise 3</h1>
        <p>If 1 = 5 , 2 = 25 , 3 = 325 , 4 = 4325 Then 5 = X - Please create new function for finding X value</p>
            <span>5 = {{ result }}</span>
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
      var arr = [
          {'id': 1, 'value' : 5},
          {'id': 2, 'value' : 25},
          {'id': 3, 'value' : 325},
          {'id': 4, 'value' : 4325},
      ]
      this.result = this.Calculate(arr)
  },
  methods : {
      Calculate(arr) {
        var _value = ''
        for( var i = arr.length; i > 0 ; i-- ) {
            _value = _value + String(i)
        }
        _value = _value.replace(1,5);
        _value = (arr.length + 1) + _value;
        return _value
      }
  }
}
</script>