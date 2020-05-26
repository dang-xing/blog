<template>
  <div>
  <a-row>
    <a-col :span="18" class="banner">
     <a-carousel :after-change="onChange" autoplay effect="fade">
        <div>
          <img src="https://www.yangqq.com/d/file/p/2019-03-04/296f82e95dd5026b6cdfacd197ae5062.png" class="banner-img"  alt="">
        </div>
        <div>
          <img src="https://www.yangqq.com/d/file/p/2019-03-04/296f82e95dd5026b6cdfacd197ae5062.png" class="banner-img"  alt="">
        </div>
        <div>
          <img src="https://www.yangqq.com/d/file/p/2019-03-04/296f82e95dd5026b6cdfacd197ae5062.png" class="banner-img" alt="">
        </div>
      </a-carousel>
    </a-col>
    <a-col :span="6" class="about">
      <div class="about-card">
          <h2>党兴的名片</h2>
          <p>职业：程序员，Web前端设计师</p>
          <p>现居：四川省-成都市</p>
          <p>工作室：青于蓝-排名技术建站</p>
          <p>Email：dancesmiling@qq.com</p>
      </div>
    </a-col>
  </a-row>
   
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
export default {
  components: {
    Logo,
  },
  methods: {
     onChange(a, b, c) {
      console.log(a, b, c);
    },
  },
}
</script>

<style scoped>
.ant-carousel >>> .slick-slide {
  text-align: center;
  height: 260px;
  overflow: hidden;
}

.ant-carousel >>> .slick-slide h3 {
  color: #fff;
}
.banner{
  box-sizing: border-box;
  padding-right: 20px;
}
.banner-img{
  width: 100%;
  height:260px;
  border-radius: 10px;
}
.about-card{
  width:100%;
  height:260px;
  background-color: rgba(42, 42, 42, 1);
  border-radius: 10px;
  box-shadow: 0px 1px 0px rgba(255,255,255,.1), inset 0px 1px 1px rgba(0,0,0,.7);
}
.about-card h2{
  font-size: 22px;
  color: #89919a;
  font-weight: normal;
  padding: 10px;
  margin:0;
  box-sizing: border-box;
}
.about-card p{
  font-size: 12px;
    padding: 0 0 0 20px;
    line-height: 28px;
    margin:0;
    text-shadow: 0px 1px 2px rgba(0,0,0,.5);
    color: #d0d2d4;
    -webkit-animation: animations2 5s ease-in-out 5s;
    -moz-animation: animations2 5s ease-in-out 5s;
    -o-animation: animations2 5s ease-in-out 5s;
    -ms-animation: animations2 5s ease-in-out 5s;
    animation: animations2 5s ease-in-out 5s;
}
</style>
