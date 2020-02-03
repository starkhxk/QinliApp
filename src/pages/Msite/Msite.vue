<template>
<section class="Home">
    <!-- 首页头部title -->
    <!-- 使用 :title 来给头部组件传递数据 -->
    <HeaderTop title="掌上沈理">
       <!--要使用slot="left"指定插入的插槽位置-->
      <router-link class="header_login" slot="left" :to="userInfo._id ? '/userinfo': '/login'">
        <span class="header_login_text" v-if="!userInfo._id">
          登录|注册
        </span>
        <span class="header_login_text" v-else>
          <i class="iconfont icon-yonghuming"></i>
        </span>
      </router-link>
        <mt-button icon="more" slot="right" style="background-color:#F3A033;"></mt-button>
    </HeaderTop> 
<div style="height:150px">
<mt-swipe :auto="4000" class=“mint-swipe” >
  <mt-swipe-item><img class="swipeimage" v-bind:src="imagurl" alt="如果我是一条鱼"/></mt-swipe-item>
  <mt-swipe-item><img class="swipeimage" v-bind:src="imagur2" alt="jdal;fja;"/></mt-swipe-item>
  <mt-swipe-item><img class="swipeimage" v-bind:src="imagur3" alt="hadsuilfha"/></mt-swipe-item>
</mt-swipe>
</div>
<div class="auto" style="margin-top: 18%;">
<mt-button  class="botton" type="primary" style="background-color:rgb(36,191,134);">
<svg t="1564652437027" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1828" width:auto height:auto><path d="M770.863 828.854c0 22.056-17.944 40-40 40H632.42l-17.553 60h115.996c55.228 0 100-44.772 100-100V686.976l-60 57.149v84.729zM176.645 828.854V390.092l186.276-186.643c11.343-11.365 10.97-29.879-0.821-40.778l-41.29-38.167h410.053c22.056 0 40 17.944 40 40v252.249l60-57.149v-195.1c0-55.228-44.772-100-100-100H255.9l-1.232-1.139-0.272 1.139h-1.875L116.645 377.635v451.219c0 55.228 44.772 100 100 100h120.853l17.553-60H216.645c-22.056 0-40-17.944-40-40z" p-id="1829" fill="#ffffff"></path><path d="M713.558 349.529c0-16.568-13.432-30-30-30H310.494c-16.568 0-30 13.432-30 30s13.432 30 30 30h373.064c16.568 0 30-13.432 30-30zM652.621 479.085c0-16.568-13.432-30-30-30H310.494c-16.568 0-30 13.432-30 30s13.432 30 30 30h312.127c16.569 0 30-13.432 30-30zM310.494 578.64c-16.568 0-30 13.432-30 30s13.432 30 30 30h219.392c16.568 0 30-13.432 30-30s-13.432-30-30-30H310.494zM892.188 496.374l-44.141-43.457c-5.074-4.675-10.775-8.321-17.156-10.992-6.381-2.621-12.866-3.956-19.403-3.956-6.537 0-13.127 1.284-19.666 3.905-6.537 2.62-12.186 6.266-16.998 10.941L495.746 726.309l116.595 116.595 279.794-274.153c10.094-9.915 15.219-21.985 15.219-36.164 0.001-14.176-5.072-26.248-15.166-36.213zM418.551 801.961L376.45 939.986l-6.695 20.649 168.304-44.946 42.174-41.324-116.592-116.593z" p-id="1830" fill="#ffffff"></path></svg>
</mt-button>
<mt-button  class="botton" type="primary" style="background-color: #F3A033;" >
  <svg t="1564650100074" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="13598" width:auto height:auto><path d="M691.85 313.571c0 15.903-11.42 28.198-26.11 28.198H266.52c-14.155 0-26.167-12.83-26.167-28.198 0-15.367 11.476-28.197 26.167-28.197h399.22c14.69 0 26.11 12.294 26.11 28.197z m0 197.72c0 15.904-11.42 28.198-26.11 28.198H266.52c-14.155 0-26.11-12.802-26.11-28.197 0-15.876 11.42-28.198 26.11-28.198h399.22c14.69 0 26.11 12.83 26.11 28.198zM466.27 708.167c0 15.903-11.42 28.705-26.11 28.705H266.52c-14.155 0-26.11-12.802-26.11-28.705 0-15.903 11.42-28.197 26.11-28.197h173.64c14.69 0 26.11 12.83 26.11 28.197z m422.624 225.749H155.761c-23.32 0-56.395-30.566-56.395-56.395V144.387c0-25.209 33.386-56.395 56.395-56.395h620.343c25.914 0 56.395 30.481 56.395 56.395v592.146c0 13.224-4.258 28.197-28.197 28.197-23.686 0-28.198-14.973-28.198-28.197V172.584c0-16.918-10.743-28.197-28.197-28.197l-560.762 2.82c-16.919 0-31.215 13.76-31.215 31.186l-0.17 670.93c0 16.918 10.744 28.197 28.198 28.197h676.739c25.913 0 28.197-2.284 28.197-28.198l-2.904-538.204c0-13.225 0.423-24.673 31.101-25.744 32.258-1.044 28.677 12.52 28.677 25.208l-0.48 566.938c0 33.78-28.648 56.395-56.394 56.395z" fill="#ffffff" p-id="13599"></path></svg>
</mt-button>
<mt-button  class="botton" type="primary" style="background-color:rgb(110,160,245)" >
  <svg t="1564650512390" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="21776" width:auto height:auto><path d="M885.76 768l-71.68 30.72c-5.12 5.12-15.36 0-15.36-10.24V240.64c0-10.24 10.24-15.36 15.36-10.24l71.68 30.72c20.48 5.12 30.72 25.6 30.72 46.08v419.84c-5.12 15.36-15.36 30.72-30.72 40.96z m-250.88-189.44c-35.84 0-66.56-30.72-66.56-71.68 5.12-30.72 25.6-51.2 56.32-56.32 15.36 0 35.84 5.12 46.08 10.24 5.12 5.12 15.36 0 15.36-5.12V163.84c0-20.48-20.48-35.84-40.96-35.84l-506.88 51.2c-20.48 0-30.72 15.36-30.72 35.84v593.92c0 20.48 15.36 35.84 30.72 35.84l506.88 51.2c20.48 0 40.96-15.36 40.96-35.84v-291.84c0-5.12-10.24-10.24-15.36-5.12-5.12 10.24-20.48 15.36-35.84 15.36z" fill="#ffffff" p-id="21777"></path></svg>
</mt-button>
<mt-button  class="botton" type="primary" style="background-color:rgb(252,129,95)">
  <svg t="1564647688002" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2841" width:auto height:auto><path d="M845.172637 265.243013c-2.718925-18.666128-18.875906-32.731472-38.169321-32.103162-20.677948 0.678452-36.912701 18.012236-36.20662 38.715767l0.444115 3.477194c0.36532 10.639315 5.1503 20.025079 12.496615 26.613124l-1.882883 2.012843c20.156062 40.364313 31.789007 85.74692 31.789007 133.927245 0 74.872245-27.736715 142.999878-73.120344 195.571211-2.665713 1.568728-5.463432 2.849908-7.763824 5.1503l-31.606859 33.096792c-0.915859 0.731664-1.725294 1.594311-2.64013 2.325975L573.473585 804.454772c0.39295-0.051165 0.784876-0.182149 1.175779-0.260943l-62.845327 65.839521-62.872956-65.839521c0.156566 0.025583 0.287549 0.053212 0.417509 0.078795L324.153216 671.12923c-5.881964-4.78498-11.346419-10.064216-16.86204-15.266705l-16.471137-17.253966c-0.207731-0.208754-0.521886-0.287549-0.731664-0.496304-47.788399-53.17406-77.197196-123.130342-77.197196-200.225207 0-165.899424 134.475737-300.402791 300.375162-300.402791 57.329706 0 110.74015 16.365736 156.304905 44.234457l0.654916-0.706081c7.137561 9.150404 18.299785 14.953573 30.795377 14.535041 20.678972-0.679475 36.887119-18.012236 36.207643-38.691207l-0.445138-3.476171c-0.522909-15.3455-10.221806-28.181853-23.606651-33.540907-58.113559-37.121456-127.051651-58.899458-201.191208-58.899458-206.813253 0-374.49016 167.652348-374.49016 374.49016 0 96.046496 36.391838 183.336562 95.864348 249.502517 1.437745 2.27481 2.484587 4.732791 4.445242 6.693446l245.686608 257.254062c0.600681 0.732687 0.836041 1.620917 1.489934 2.248204 3.660366 3.660366 7.894807 6.431479 12.417821 8.261151 13.907755 6.535857 30.874171 4.444219 42.376133-7.057743 2.955308-2.980891 4.862751-6.483668 6.614651-9.987468L785.776875 691.62503c1.515516-1.51654 2.196015-3.451612 3.397377-5.124717 60.337203-66.349127 97.327676-154.265456 97.327676-251.072269C886.501928 374.047068 871.417371 316.324412 845.172637 265.243013zM360.465237 437.5995c0 83.603093 67.76129 151.364383 151.365406 151.364383 83.576487 0 151.36336-67.76129 151.36336-151.364383S595.40713 286.234093 511.830643 286.234093C428.226526 286.234093 360.465237 353.996406 360.465237 437.5995zM585.916988 437.049984c0 41.22696-33.408901 74.66349-74.636884 74.66349-41.252543 0-74.662467-33.43653-74.662467-74.66349 0-41.225937 33.409924-74.662467 74.662467-74.662467C552.508088 362.387517 585.916988 395.824047 585.916988 437.049984z" p-id="2842" fill="#ffffff"></path></svg>
</mt-button>
</div>
<div style="padding-top:5px">
<p class="auto"><span>考试信息</span><span>在线笔记</span><span>教室申请</span><span>新生报道</span></p>
</div>
<br>
<br>
<div style="padding-top:5px">
<div class="middleone">
            <ul class="nav">
              <!-- <li class="limited" v-for="value in mesgArrays" :key="value">
                <ronter-link to="/" tag="a">
                <a>{{mesgArrays.name}}</a>
              </ronter-link>
              </li> -->
                <li class="limited">
                    <a href="#">这是一条教务通知信息科学技术与工程学院做</a>
                </li>
                <li class="limited">
                    <a href="#">这是一条教务通知信息科学技术与工程学院做</a>
                </li>
                <li class="limited">
                    <a href="#">这是一条教务通知信息科学技术与工程学院计算机科学与技术</a>
                </li>
                <li class="limited">
                    <a href="#">这是一条教务通知信息科学技术与工程学院</a>
                </li>
                <li class="limited">
                    <a href="#">这是一条教务通知信息科学技术与工程学院</a>
                </li>
            </ul>
            <div class="logo">
                <a href="#" title="这是个很好的logo">
                  <strong>
                <p style="font-family:FZShuTi;font-size:22px;color:#F3A033">教务</p>
                <p style="font-family:FZShuTi;font-size:22px;color:#F3A033">通知</p>
                </strong></a>
            </div>
        </div>
</div>
<div>
<h5 style="padding: 3%;padding-top:37px;color:#808080;font-family:FZShuTi;font-size:22px">报告会</h5>
</div>
<div class="report">
<div class="yuanjiao">
  <!-- 左列 -->
        <div class="li-left">
            <ul>
                <li>时间：2019/10/23</li>
                <li>地点：信息科学与工程学院A302</li>
                <li>主讲人：曲铁平教授</li>
            </ul>
        </div>
        <!-- 右列 -->
        <div class="li-right">
            <ul>
                <li class="li-tip">主题:线性代数</li>
                <br>
                <li><img class="img-report" src="./images/qrcode_1554361539952.jpg" alt="报告会插图" align="top"></li>
            </ul>
        </div>
</div>
    </div>
</section>
</template>

<script>
import 'mint-ui/lib/style.css'
// 引入头部组件
import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
import {mapState} from 'vuex'
import ajax from '../../api/ajax'
export default {
  data () {
    return {
      mesgArrays: [
        { name: 'Runoob' },
        { name: 'Google' },
        { name: 'Taobao' }
      ],
      imagurl: require('./images/swipeone.jpg'),
      imagur2: require('./images/swipetwo.jpg'),
      imagur3: require('./images/swipethree.jpg')
    }
  },
  components: {
    HeaderTop
  },
  computed: {
    ...mapState(['userInfo']),
  },
  created: {
  },
  mounted () {
    this.getDate()
  },
  methods: {
    // async getDate(){
    //   const data=await getselSchoolTimeTable('1803050128','2019-2020','1');
    //   console(data);
    // },
    getDate () { 
      console.log("shuchu ")
        let data=ajax('http://localhost:8081/api/selSchoolTimeTable',
      {
        XH:'1803050120',
        XN:'2019-2020',
        XQ:'1'
      },
      'GET'
      )
      console(data);
    },
    /**
    getTest(){
      var ajax = new XMLHttpRequest();
//步骤二:设置请求的url参数,参数一是请求的类型,参数二是请求的url,可以带参数,动态的传递参数starName到服务端
      ajax.open('get','http://ql.sylu.edu.cn/qlapp/selSchoolTimeTable?XH=1803050120&XN=2019-2020&XQ=1');
//步骤三:发送请求
      ajax.send();
//步骤四:注册事件 onreadystatechange 状态改变就会调用
      ajax.onreadystatechange = function () {
   if (ajax.readyState==4 &&ajax.status==200) {
    //步骤五 如果能够进到这个判断 说明 数据 完美的回来了,并且请求的页面是存在的
　　　　console.log(ajax.responseText);//输入相应的内容
  　　}
    }
    },*/
    initData () {
      console.log(this.mesgArrays)
      // for(var i=1;i<mesgArrays.length;i++)
      // console.log(mesgArrays[i].name);
    }
  }
}
</script>

<style>
/* .Home{
  width: 100%;
  overflow: scroll;
} */
.mint-swipe{
  padding-top: 46px;
  height:100%;
  width:100%;
  }
.swipeimage{
  max-width:100%;
  max-height:100%;
}
.botton{
    height:60px;
    width: 60px;
    --color:#ffffff;
    background-color: #F3A033;
    border-radius: 25px;
}
    .middleone{
        padding-top: 0px;
        width: 100%;
        margin: 0 auto;
        height: 60px;
    }
    .nav li{
        list-style: none;
    }
    .logo{
        padding-top: 20px;
        margin-left:5%;
    }
    .nav{
        /* padding-top: 60px; */
        padding-right: 5%;
        padding-left: 5%;
        /* padding-bottom: 60px; */
        border-left: 2px black dotted;
        float: right;
        width: 68%;
    }
    .nav a{
    font-size:10px;
    color: #666;
    text-decoration: none;
}
.nav a:hover{
    color: #b7b7b7;
    text-decoration: underline;
}
.limited{
  width: 98%;
  overflow: hidden;     /*内容超出后隐藏*/
  text-overflow: ellipsis;    /*超出部分为省略号*/
  white-space: nowrap;     /*文本不进行换行*/
}
.auto{
  font-size:11px;
  display:flex;
  justify-content: space-around;
  width: 100%;
  margin: 0 auto;
}
/* .report{
  border-radius:60px;
  width:87%;
  height:150px;
  border:#900 1px solid;
  margin-right: 10%;
  margin-left: 7%;
  margin-bottom: 53px;
} */
.yuanjiao{
    background: #ffffff;
    border-radius:50px;
    padding:10px;
    border: 1px solid #eb5656;
    width:80%;
    margin: auto;
    margin-bottom: 18%;
    height:180px;
}
.li-left{
    float: left;
    /* background-color: #eb5656; */
    width: 50%;
    height: 100%;
    border-radius:50px;
    text-align: center;
    padding-top: 30px;
    line-height: 2;
}
.li-right{
    float: left;
    /* background-color:#63ddd3; */
    width: 50%;
    height: 100%;
    border-radius:50px;
    text-align: center;
    padding-top: 30px;
    line-height: 2;
}
.img-report{
width: 50px;
height: 50px;
}
.li-tip{
font-weight:800;
}
</style>
