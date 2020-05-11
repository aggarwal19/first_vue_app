<template>
  <div>
    <p>Enter a number:</p> 
    <input type="number" v-model.number="age" />
    <br/>
    <button class="btn" v-on:click="valid">submit</button>
    <br/>
    <p> entered number is:{{age}}</p>
    <p>Cube is: {{cube}}</p>
    <p>{{error}}</p>
  </div>
</template>

<script>
export default {
  name: 'firstfile',
  data: function(){
    return{
      age : 0,
      cube : 0,
      error:null
    }
  },
  methods:{
    valid : function()
      {
        var n = this.age;
        if(typeof(n)=="number")
        {
          this.cube = n*n*n;
          this.error = null;
        }
        else
        {
          this.cube = "not possible";
          this.error = "Error is : only numeric value is allowed";
        }
      }
  }
}



</script>

<style scoped>
input {
  margin-left: 10px;
  padding:20px
}
.btn{
  padding:10px;
  margin: 10px;
}
</style>