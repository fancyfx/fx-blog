<template>
  <div class="hello">
    <div class="logo mar_bot">
      <img src="../assets/fancyxi.png">
    </div>
    <div class="title mar_bot">
      <h1>{{ msg }}</h1>
    </div>
    
    <div class="title_description mar_bot">
      <h2>hi，你好！我是方希(@fancyxi).</h2>
    </div>
    
    <div class="link_button mar_bot">
        <ul>
          <li><a href="#" target="_blank">博客</a></li>
          <li><a href="#" target="_blank">记事本</a></li>
          <li><a href="#" target="_blank">项目</a></li>
          <li><a href="#" target="_blank">关于</a></li>
        </ul>
    </div>
    <div class="link_icon mar_bot">
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
      msg: "Fancyxi's Blog",
    };
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
}
.mar_bot {
  margin-bottom: 20px;
}
.link_button{
  margin-top: 20px;
}
.link_icon{
  margin-top: 20px;
}
</style>
