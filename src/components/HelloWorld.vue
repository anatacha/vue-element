<template>
  <div class="hello">
       <el-button @click="visible = true" style="border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);">Button</el-button>
    <el-dialog :visible.sync="visible" title="Hello world">
      <p>Try Element</p>
      <el-form   label-width="120px">
         <el-form-item label="Activity name">
            <el-input></el-input>
        </el-form-item>
      </el-form>
    </el-dialog>
        
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
   data: function(){
    return {visible:false}
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
