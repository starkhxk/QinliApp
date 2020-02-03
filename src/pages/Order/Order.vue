<template>
<section class="ScheduleCard">
<div>
    <section class="order">
      <HeaderTop title="课程表"></HeaderTop>
    </section>
    <div class="topone">
        <button class="bt1">5</button>
        <button class="bt2">5</button>
        <div>第十周</div>
    </div>
    <div class="middle">
        <div class="bigCommon p1">
                <div class="smallCommon one1">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon one2">
                    <div class="contentUp">
                        <p>大学英语</p>
                    </div>
                    <div class="contentDown">
                        <p> A-119</p>
                    </div>
                </div>
                <div class="smallCommon one3">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon one4">
                    <div class="contentUp">
                        <p>招贴设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-328</p>
                    </div>
                </div>
                <div class="smallCommon one5">
                    <div class="contentUp">
                        <p>马克思主义基本原理概论</p>
                    </div>
                    <div class="contentDown">
                        <p> A-409</p>
                    </div>
                </div>
        </div>
        <div class="bigCommon p2">
                <div class="smallCommon two1">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon two2">
                    <div class="contentUp">
                        <p>大学英语</p>
                    </div>
                    <div class="contentDown">
                        <p> A-119</p>
                    </div>
                </div>
                <div class="smallCommon two3">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon two4">
                    <div class="contentUp">
                        <p>招贴设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-328</p>
                    </div>
                </div>
                <div class="smallCommon two5">
                    <div class="contentUp">
                        <p>马克思主义基本原理概论</p>
                    </div>
                    <div class="contentDown">
                        <p> A-409</p>
                    </div>
                </div>
        </div>
            <div class="line">
            </div>
        <div class="bigCommon p3">
                <div class="smallCommon three1">
                    <div class="contentUp">
                        <p>马克思主义基本原理概论</p>
                    </div>
                    <div class="contentDown">
                        <p> A-409</p>
                    </div>
                </div>
                <div class="smallCommon three2">
                    <div class="contentUp">
                        <p>大学生职业发展与创业就业指导</p>
                    </div>
                    <div class="contentDown">
                        <p> A-210</p>
                    </div>
                </div>
                <div class="smallCommon three3">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon three4">
                    <div class="contentUp">
                        <p>CI设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-407</p>
                    </div>
                </div>
                <div class="smallCommon three5">
                    <div class="contentUp">
                        <p>大学生职业发展与创业就业指导</p>
                    </div>
                    <div class="contentDown">
                        <p> A-210</p>
                    </div>
                </div>
        </div>
        <div class="bigCommon p4">
                <div class="smallCommon four1">
                    <div class="contentUp">
                        <p>马克思主义基本原理概论</p>
                    </div>
                    <div class="contentDown">
                        <p> A-409</p>
                    </div>
                </div>
                <div class="smallCommon four2">
                    <div class="contentUp">
                        <p>篮球</p>
                    </div>
                    <div class="contentDown">
                        <p> X-xxx</p>
                    </div>
                </div>
                <div class="smallCommon four3">
                    <div class="contentUp">
                        <p>动态网络设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-406</p>
                    </div>
                </div>
                <div class="smallCommon four4">
                    <div class="contentUp">
                        <p>CI设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-407</p>
                    </div>
                </div>
                <div class="smallCommon four5">
                    <div class="contentUp">
                        <p>大学生职业发展与创业就业指导</p>
                    </div>
                    <div class="contentDown">
                        <p> A-210</p>
                    </div>
                </div>
        </div>
        <div class="bigCommon p5">
                <div class="smallCommon five1"></div>
                <div class="smallCommon five2"></div>
                <div class="smallCommon five3"></div>
                <div class="smallCommon five4">
                <div class="contentUp">
                        <p>CI设计</p>
                    </div>
                    <div class="contentDown">
                        <p> C-407</p>
                    </div>
                </div>
                <div class="smallCommon five5"></div>
        </div>
    </div>
  </div></section>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
export default {
  components: {
    HeaderTop
  }
}
</script>

<style type="text/css">
.ScheduleCard{
  width: 100%;
  overflow: scroll;
}
        .topone{
            width: 31%;
            margin: 20px auto;
            text-align: center;
            color: rgb(119, 110, 111);
            padding-top: 40px;
        }
        /* 设置按钮大小 */
        .bt1{
            width: 20px;
            float: left;
        }
        .bt2{
            width: 20px;
            float: right;
        }
        /* 设置课表高度 */
    .middle{
        margin: 0 auto;
        height: 400px;
    }
    /* 设置每一行课表 */
    .middle .bigCommon{
        height: 25%;
        margin-top: 3%;
    }
    .middle .p2{
        margin-bottom: 3%;
    }
    .line{
        height: 1px;
        background: radial-gradient(rgb(224,224,224) 24%, white 100%);
    }
    /* 课表框 */
    .bigCommon div{
        width: 16%;
        height: 100px;
    }
    .smallCommon{
        float: left;
        margin: 0 2%;
        text-align: center;
        border-radius: 10px;
        font-size: 10px;
        color: rgb(255, 249, 253)
    }
    .smallCommon .contentUp{
        width: 100%;
        position: relative;
        top: 6px;
        left: 0px;
    }
    .smallCommon .contentDown{
        width: 100%;
        position: relative;
        bottom: 25px;
        left: 0px;
    }
    .one1{
        background-color: rgb(250, 122, 85);
    }
    .one2{
        background-color: rgb(254, 173, 21);
    }
    .one3{
        background-color: rgb(250, 122, 85);
    }
    .one4{
        background-color: rgb(102, 156, 244);
    }
    .one5{
        background-color: rgb(117, 102, 243);
    }
    .two1{
        background-color: rgb(250, 122, 85);
    }
    .two2{
        background-color: rgb(254, 173, 21);
    }
    .two3{
        background-color: rgb(250, 122, 85);
    }
    .two4{
        background-color: rgb(102, 156, 244);
    }
    .two5{
        background-color: rgb(117, 102, 243);
    }
    .three1{
        background-color: rgb(117, 102, 243);
    }
    .three2{
        background-color: rgb(36, 191, 134);
    }
    .three3{
        background-color: rgb(250, 122, 85);
    }
    .three4{
        background-color: rgb(254, 146, 146);
    }
    .three5{
        background-color: rgb(36, 191, 134);
    }
    .four1{
        background-color: rgb(117, 102, 243);
    }
    .four2{
        background-color: rgb(173, 91, 43);
    }
    .four3{
        background-color: rgb(250, 122, 85);
    }
    .four4{
        background-color: rgb(254, 146, 146);
    }
    .four5{
        background-color: rgb(36, 191, 134);
    }
    .five1,.five2,.five3,.five5{
        background-color: rgb(235, 233, 234);
    }
    .five4{
        background-color: rgb(254, 146, 146);
    }
    </style>
