<template>
  <div id="app">
    <Navbar></Navbar>
    <div class="main-section-container">
      <img class="vuejs-logo" src="./images/Vue_logo.png" alt="vuejs-logo">
      <h1>Welcome to Vue.js</h1>
      <h3>Become a coding ninja with the fastest- <br> growing JavaScript framework</h3>
      <button>Awesome!</button>
    </div>
  </div>
  <div class="footer-container">
    <div class="item">
      <img src="./images/USP-1.png" alt="">
      <h5>Performant</h5>
      <p>Truly reactive, compiler-optimized rendering <br> system that rarely <br> requires manual <br> optimization.</p>
    </div>
    <div class="item">
      <img src="./images/USP-2.png" alt="">
      <h5>Approachable</h5>
      <p>Builds on top of standard <br> HTML, CSS and JavaScript <br> with intuitive API and <br> world-class <br> documentation.</p>
    </div>
    <div class="item">
      <img src="./images/USP-3.png" alt="">
      <h5>Versatile</h5>
      <p>A rich, incrementally <br> adoptable ecosystem <br> that scales between a <br> library and a full- <br>featured framework.</p>
    </div>
  </div>
</template>

<script>
  import Navbar from "./components/navbar.vue"
  export default {
    name: 'App',
    components:{
      Navbar
    }
  }
</script>

<style>
  body{
    margin: 0px;
  }
  #app{
    width:100%;
    height:100%;
    display: flex;
    flex-direction: column;
    gap: 100px;
  }
  .main-section-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family:Arial, Helvetica, sans-serif;
    text-align: center;
  }
  .main-section-container h1{
    font-size: 75px;
    margin-top: 10px;
    margin-bottom: 15px;
  }
  .main-section-container h3{
    font-size: 25px;
    margin-top: 0px;
    margin-bottom: 30px;
  }
  .main-section-container button{
    background-color: rgba(52, 73, 94, 1);
    width: 170px;
    height: 40px;
    border-radius: 50px;
    color: white;
    font-size: 20px;
  }

  .vuejs-logo{
    width: 230px;
  }
  .footer-container{
    background: rgba(57, 185, 131, 1);
    display: flex;
    flex-direction: row;
    justify-content:center;
    align-items: center;
    gap: 75px;
    padding-top: 150px;
    padding-bottom: 100px;
  }
  .item{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    width: 250px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 500;
  }
  .item h5{
    font-size: 30px;
    margin: 0px;
    margin-top: 25px;
  }
  .item p{
    font-size: 20px;
    margin-top: 30px;
  }
  .item img{
    width: 95px;
  }
</style>