<template>
  <div class="hello">
    {{aaa.value}}
    <div @click='btnclick'>按钮</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return {
      aaa:{
        value:"yanzhang"
      }
    }
  },
  props: {
    msg: String,
  },
  methods:{
    btnclick(){
      this.aaa.value = 'bbb';
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
