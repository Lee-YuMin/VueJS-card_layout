<template>
  <div class="container">
  <h1>{{$route.params.id}}</h1>
  </div>
</template>

<script>
export default {
  name: 'Detail',
  data () {
    return {
      arr: [],
      id: '1'
    }
  },
  created: function() {
  
  },
  methods: {
    clickShare: function(title) {
      console.log(title)
    }
  }
}
</script>
<style scoped>
ul {
  list-style:none;
}
span{
    font-size:15px;
}
a{
  text-decoration:none; 
  color: #0062cc;
  border-bottom:2px solid #0062cc;
}
.box{
    padding:60px 0px;
}

.box-part{
    background:#FFF;
    border-radius:0;
    padding:60px 10px;
    margin:30px 0px;
}
.text{
    margin:20px 0px;
}

.fa{
     color:#4183D7;
}
</style>