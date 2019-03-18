<style scoped>

.container {
  background: #eee;
}
ul {
  list-style:none;
}
li {
  min-width: 200px;
}
span{
    font-size:15px;
}
a {
  text-decoration:none; 
  color: #000;
  border-bottom:2px solid #0062cc;
}
a:hover {
  color: #0062cc;
  cursor:pointer;
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
.icon { 
  width: 50px;
  height: 50px;
}
</style>

<template>
  <div class="box">
    <div class="container">
      <ul>
        <li v-for="item in items" :key="item.id">
          <a v-on:click="gotoDetail(item)">
            <div class="col-lg-4 col-md-4"> 
              <div class="box-part text-center">
                  <img src="../assets/job_icon.png" class="icon">
                  <div class="title">
                    <h4>{{item.title}}</h4>
                  </div>         
                  <div class="text">
                    <div>회사명 : {{item.company}}</div>
                    <div>모집분야 : {{item.skill}}</div>
                    <div>경력 : {{item.years}}</div>
                    <div>페이 : {{item.price}}</div>
                    <div>위치 : {{item.location}}</div>
                  </div>
                </div>
              </div>
            </a>
          </li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'List',
  data () {
    return {
      items: []
    }
  },
  created: function() {
    this.items.push({
      id: 'aaa',
      title: "AAA회사의 공채를 모집합니다.",
      company: "(주)AAA",
      years: 0,
      price: "3500",
      skill: "신입",
      location: "서울특별시 강남구 OO동 ABC빌딩"
    },{
      id: 'bbb',
      title: "BBB회사의 프론트엔드 개발자를 모집합니다.",
      company: "(주)BBB",
      years: "3년이상",
      price: "3000~3500",
      skill: "프론트엔드",
      location: "서울특별시 강남구 XX동 DEF빌딩"
    },{
      id: 'ccc',
      title: "CCC에서 백엔드 PM급 모십니다.",
      company: "(주)CCC",
      years: "5~7년",
      price: "협의",
      skill: "백엔드 PM급?",
      location: "서울특별시 강남구 QQ동 GHI빌딩"
    },{
      id: 'ddd',
      title: "DDD에서 누구든 구합니다.",
      company: "(주)DDD",
      years: "무관",
      price: "협의",
      skill: "아무나...",
      location: "서울특별시 강남구 TT동 OTL빌딩"
    })
  },

  methods: {
    gotoDetail: function(item) {
      window.location.hash = `#/detail/${item.id}`;
    }
  }
}
</script>
