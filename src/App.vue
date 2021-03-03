<template>
<div class="resume">
  <div class="top">	</div>
  <div class="left">
    <h1>林姿瑩</h1>
    <h4 class="sc">高雄科技大學 | 海事資訊系</h4>
    <h2>自我介紹</h2>
    <div class="buttons">
      <a class="btn fill" href=" " target="_blank">相關連結</a>
      <a class="btn nonefill" href=" " target="_blank">個人收集</a>
    </div>
    <div class="block">
      <h2>學業成就</h2>
      <ul class="ListExperience">
        <li class="year">2006-2012
          <ul><li>右昌國小 </li></ul>
        </li>
        <li class="year">2012-2014
          <ul><li>右昌國中 </li></ul>
        </li>
        <li class="year">2014-2016
          <ul><li>鳳商商工-商業經營科 </li></ul> 
        </li> 
        <li class="year">2016-2020
          <ul><li>高雄科技大學-海事資訊系 </li></ul> 
        </li> 
      </ul>
    </div>    
  </div> 
    
  <div class="right">
    <div class="decoration"></div>
    <div class="block">
      <h2>專業技能</h2>
      <ul class="listSkill">
        <li>
          <div class="circle a">
            <div class="p90"></div>
            <div class="p180"></div> 
            <div class="p270"></div>
          </div>
        </li>
        <li>
          <div class="circle b">
            <div class="p90"></div>
            <div class="p180"></div>
          </div>
        </li>
        <li>
          <div class="circle c">
            <div class="p90"></div>
          </div>  
        </li>
      </ul>
    </div>
    <div class="block">
      <h2>專業證照</h2>
      <ul class="listProgram">
        <li>門市服務
          <div class="bar">
            <div class="value p95"></div>
          </div>
        </li>
        <li>會計事務-人工
          <div class="bar">
            <div class="value p80"></div>
          </div>
        </li>
        <li>會計事務-資訊
          <div class="bar">
            <div class="value p80"></div>
          </div>
        </li>
        <li>電腦軟體應用
          <div class="bar">
            <div class="value p60"></div>
          </div>
        </li>
      </ul>
    </div>
    <div class="photo"></div>
  </div>
</div>
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

  .left *{
    margin:0px;
  }

  .resume{
    font-family:"標楷體";
    width:800px;
    height:1000px;
    display:flex;
    position:relative;
  }

  .top{
    width:100%;
    height:250px;
    display:flex;
    background-size: cover;
    position:absolute;
    background-image: url(https://assets2.razerzone.com/images/pnx.assets/3a52f8b4de652b09ce8a3cf2108622f3/campaigns-quartz-hero-mobile-update.jpg);
    background-size: cover;
    background-position:center;
    align-items:center;
    justify-content:center;
  }

  body{
  /* 	background-size: cover; */
    padding:30px;
    justify-content:center;
    display:flex;
    color:#626262;
    font-family: 'Indie        Flower', cursive;
  /* 	中文字寬度調整 */
    line-height:28px;
    letter-spacing:0.5px;
    background-color: #403F45;
  }

  .left{
    position: relative;
    flex:8;
    padding-right:15px;
    background-color:#F7B8BC;
    /* 	透明度 */
    color:rgba(64,64,64,0.95); 
  }

  .right{
    position: relative;
    flex:8;
    padding-left:25px;
    background-color:white;
  }

  .right,.left{
    padding:15px;
    margin-top:250px;
    margin-bottom:70px;
  }

  a{
    text-decoration:none;
  }

  .buttons .btn{
    border-radius:50px;
    overflow:hidden;
    transition:0.7s;
    padding: 5px 25px;
    margin-top:15px;
    margin-bottom:15px;
  }

  .buttons{
    margin-bottom:60px;
  }

  .fill:hover{
    background-color: #F7E8B8;
  }

  .nonefill:hover{
    background-color: #F7E8B8;
  }

  /* 編輯ul,il的畫面 */
  ul{
    padding:0;
    list-style:none;
  }

  .fill{
    float:left;
    margin-left:20px;
    color:#7F7676;
  }

  .nonefill{
    float:right;
    margin-right:20px;
    color:#7F7676;	
  }

  /* h2::after{
    content:"";
    display:inline-block;
    width:10px;
    height:20px;
    background-color: #EF9F96;
    margin-left:10px;
    padding-bottom:2px;
  } */

  .left>h2 ,.left>.block>h2{
    background-color: #fff;
    font-size:20px;
    padding-left:5px;
    padding-top:5px;
    font-weight:100;
    width:90px;
    border-top-left-radius:10px;
    border-top-right-radius:10px;
    position: relative;
  /* 	字體柔和 */
  }	

  .right>.block>h2,.right>h2{
    background-color: #EF9F96;
    font-size:20px;
    padding-left:8px;
    padding-top:5px;
    font-weight:100;
    width:90px;
    border-top-left-radius:10px;
    border-top-right-radius:10px;
    position: relative;
  }

  .left > h2 + div::before, 
  .left > .block > h2 + ul:before{
      position: absolute;
      background-color: white;
      display: block;
      width: calc(100% - 30px);
      height: 3.5px;
      content: "";
  }

  .right > .block > h2 + ul::before{
      position: absolute;
      background-color: #EF9F96;
      display: block;
      width: calc(100% - 30px);
      height: 3.5px;
      content: ""
  }

  h4{
    margin-top:30px;
    padding-top:25px;
    opacity:0.8;
    font-weight:100;
  }

  .ListExperience li ul{
    padding-left:15px;
    border-left:solid 2px #8c8c8c;
    margin-left: 10px;
    /*補上面的 margin-bottom*/  
  }

  .circle{
    width: 80px;
    height: 80px;
    margin-top:16px;
    margin-bottom:16px;
    background-color: white;
    border-top-right-radius:5px;
    border-bottom-right-radius:5px;
    border-bottom-left-radius-radius:5px;
  /*   border-radius:50%; */
    position: relative;
    /*p90超過的要藏起來*/
    overflow:hidden;
  }

  .p90{
    width:50%;
    height:50%;
    position: absolute;
    left:50%;
    top:0;
    background-color: #EF9F96;  
  }

  .p180{
    width:50%;
    height:50%;
    position: absolute;
    /*距離左邊*/
    left:50%;
    /*距離上方*/
    top:50%;  
    background-color: #EF9F96;  
  }

  .p270{
    width:50%;
    height:50%;
    position: absolute;
    left:0;
    top:50%;
    background-color: #EF9F96; 
  }

  .circle::after{
    content:"";
    display:block; /*設定寬高*/
    background-color: white;
    width:calc(100% - 13px);
    height:calc(100% - 13px);
  /*   border-radius:50%; */
    position: relative;
    left:50%;
    top:50%;
    transform:translate(-50%,-50%);				color:black;
    align-content:center;
    line-height:67px;
  }
  .a.circle::after{
    content:"HTML";
  }

  .b.circle::after{
    content:"CSS";
  }

  .c.circle::after{
    content:"JS";
  }

  .listSkill{
    display:flex;
    flex-wrap:wrap;
  }

  .listSkill li{ 
    width:30%;
    padding:5px;
    box-sizing:border-box;
    display:flex;
    flex-direction:column;
    /*沒有反應 因為排列所以上去補 display:flex*/
    /*圖片致中*/
    align-items:center;
    /*文字致中*/
    text-align:center;   
  }

  .sc{
    margin-bottom:15px;
  }

  .right > .block > h2{
  margin-bottom:0px;
  }

  .right > .block > h2 + ul{
  margin-top:0px;
  }

  .listSkill li,.listProgram li{
      padding-top: 20px;
  }

  .decoration{
    width: 300px;
    height: 50px;
    background:linear-gradient(90deg,#F7B8BC,#ffcbc2,#ffffff);
  /*   border-radius:70px; */
    border-radius:0px 90px 90px -50px;
    position:absolute; /*resume*/
    left:0;
    bottom:0;  
  }

  .photo{
    width:75px;
    height:75px;
    background-image: url(http://tw.mensuno.asia/sites/default/files/17836656_1520756504601717_952579305_o.jpg);	
    border-radius:50%;
    position:absolute;
    background-size: cover;
    left:-30px;
    bottom:20px;
    transition:2s;
  }

  .listSkill li{ 
    width:30%;
    padding:5px;
    box-sizing:border-box;
    display:flex;
    flex-direction:column;
    /*沒有反應 因為排列所以上去補 display:flex*/
    /*圖片致中*/
    align-items:center;
    /*文字致中*/
    text-align:center; 
  }

  .listProgram .bar{
    width:80%;
    height:15px;
    border:solid 2px #EF9F96;
    margin-bottom:-15px;
    border-radius:25px;
    overflow:hidden;
    
  }
  .value{
    height:100%;
    width:50%;
    background-color: rgb(255, 203, 194); 
  }

  .value.p10{
    width:10%;
  }

  .value.p95{
    width:90%;
  }

  .value.p60{
    width:60%;
  }
  .value.p80{
    width:80%;
  }

  .photo:hover{
    box-shadow:0px 0px 35px rgba(0,0,0,0.5);
  /* 游標移動的時候card會移動	 */
    transform:translate(0px,-500px);
  }
</style>
