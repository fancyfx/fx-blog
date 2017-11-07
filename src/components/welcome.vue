<template>
  <div class="hello" v-bind:class="{ home_hellp: toHomeStyle.isHome }">
    <div class="logo mar_bot">
      <img src="../assets/fancyxi.png">
    </div>
    <div class="title">
      <h1>{{ welMsg.title }}</h1>
    </div>
    <hr class="panel-cover__divider">
    <div class="title_description mar_bot" v-bind:class="{ home_title_description: toHomeStyle.isHome }">
      <p>{{ welMsg.description }}</p>
    </div>
    
    <div class="link_button ">
        <ul>
          <li><a href="" target="_blank" v-on:click.stop.prevent="toHomeStyle.isHome = !toHomeStyle.isHome">博客</a></li>
          <li><a href="#" target="_blank">记事本</a></li>
          <li><a href="#" target="_blank">项目</a></li>
          <li><a href="#" target="_blank">关于</a></li>
        </ul>
    </div>
    <div class="link_icon ">
      <ul>
        <li><a href="#" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a></li>
        <li><a href="#" target="_blank"><i class="fa fa-envelope" aria-hidden="true"></i></a></li>
        <li><a href="#" target="_blank"><i class="fa fa-weixin" aria-hidden="true"></i></a></li>
        <li><a href="#" target="_blank"><i class="fa fa-rss" aria-hidden="true"></i></a></li>  
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data() {
    return {
      welMsg: {
        title: "Fancyxi's Blog",
        description: 'Hi，你好！我是方希(@fancyxi),是一名前端开发者！现在工作生活于武汉。我对后端开发也比较熟悉，写过nodejs、php、java等。由于工作的经历，我对HTTP协议和WEB安全有一定研究.',
      },
      toHomeStyle: {
        isHome: false,
      },
    };
  },
  methods: {
    toHome() {
      this.toHomeStyle.isHome = !this.toHomeStyle.isHome;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import "~font-awesome/css/font-awesome.min.css";
h1, h2 {
  font-weight: normal;
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
  color: #000;
  text-decoration:none;
}
.logo img{
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 3px solid #FFF;
  box-shadow: 0 0 1px 1px rgba(0, 0, 0, 0.3);
}
.link_button a{
    color: #42b983;
    padding: 10px 20px;
    border: 1px solid #42b983;
    border-radius: 20px;
    font-size: .9em;
    font-weight: bold;
    letter-spacing: 1px;
    text-shadow: none;
    -webkit-font-smoothing: antialiased;
}
.hello {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction:column;
    flex-wrap: nowrap;
    align-items:center;
    justify-content: center;
}
.fa {
  font-size: 28px;  
  color: #333333;
}
.link_button{
  margin-top: 20px;
  margin-bottom: 40px;
}
.link_icon{
  margin-top: 20px;
}
.title_description{
  text-align: center;
  width: 600px;
  margin-bottom: 40px;
}
.home_title_description{
  width: 80%;
}
.title_description>p {
  font-size: 18px;
  line-height: 30px;
}
.panel-cover__divider{
    width: 20%;
    margin: 20px auto;
    border-top: 1px solid #bbb;
  }
  .hello {
    background-color: #eee;
  }
  .home_hellp {
    width: 30%;
  }
</style>
