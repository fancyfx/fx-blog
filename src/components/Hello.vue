<template>
  <div class="hello">
    <div class="logo">
      <img src="../assets/fancyxi.png">
      <h1>{{ msg }}</h1>
    </div>
      
    <div class="description">
      <h2>hi，你好！我是方希(@fancyxi).</h2>
    </div>
    
    <div class="link">
      <div class="blog-button" >
        <ul>
          <li><a href="#" target="_blank">博客</a></li>
          <li><a href="#" target="_blank">记事本</a></li>
          <li><a href="#" target="_blank">项目</a></li>
          <li><a href="#" target="_blank">关于</a></li>
        </ul>
      </div>
      <div>
        <i class="fa fa-address-book" aria-hidden="true"></i>
      </div>
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
  color: #42b983;
  text-decoration:none;
}
.logo img{
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 3px solid #FFF;
  box-shadow: 0 0 1px 1px rgba(0, 0, 0, 0.3);
}
.blog-button a{
    padding: 10px 20px;
    border: 1px solid #42b983;
    border-radius: 20px;
    font-size: .9em;
    font-weight: bold;
    letter-spacing: 1px;
    text-shadow: none;
    -webkit-font-smoothing: antialiased;
}
</style>
