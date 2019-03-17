<template>
  <div class="panel panel-default">
    <ul>
      <li>
        <div class="col-lg-4 col-md-4 col-sm-4 col-xs-12"> 
            <div class="box-part text-center">
              <i class="fa fa-instagram fa-3x" aria-hidden="true"></i>
                          
              <div class="title">
                <h4>Instagram</h4>
              </div>
                          
              <div class="text">
                <span>Lorem ipsum dolor sit amet, id quo eruditi eloquentiam. Assum decore te sed. Elitr scripta ocurreret qui ad.</span>
              </div>
                          
              <a href="#">Learn More</a>
                          
              </div>
          </div>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'List',
  data () {
    return {
      msg: 'Basic panel example'
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