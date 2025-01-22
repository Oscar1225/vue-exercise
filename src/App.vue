<template>
    <div>
        <ContainerComponent />
    </div>
    <br>
    <div>
        <ContainerComponent2/>
    </div>
      <br>
    <div class="container3">
        <a href="#" class="b">Home</a>
        <a href="#" class="b">Payment</a>
        <a href="#" class="b">Paymddent</a>
        <a href="#" class="b">Customer</a>
        <a href="#" class="b">Products</a>
        <a href="#" class="b">Reports</a>
        <a href="#" class="b3">Connect</a>
        <select name="More" id="More" class="more b5">
            <option value="">More</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
        </select>
        <a href="#" class="b3">Developers</a>
        <label class="b3">
            <input type="checkbox" name="" id="" class="checkbox">
            <span class="btn-box">
                <span class="btn">
                </span>      
            </span>
            <span class="text">Test Mode</span>
        </label>
        </div>
        <br>
    <div class="wrapper">
        <div class="container4">
            <h1 class="title">Activate account</h1>

            <span class="c1">
                <h2 class="c2">step1</h2>
                <h2>Contact Information</h2>
                <h2>in progress</h2>
            </span>

            <span class="c1">
                <h2 class="c2">step2</h2>
                <h2>Business Information</h2>
                <h2>in progress</h2>
            </span>

            <span class="c1">
                <h2 class="c2">step3</h2>
                <h2>Banking Information</h2>
                <h2>in progress</h2>
            </span>

            <span class="c1">
                <h2 class="c2">step4</h2>
                <h2>Ownership Information</h2>
                <h2>in progress</h2>
            </span>

            <span class="c1">
                <h2 class="c2">step5</h2>
                <h2>Terms & Information</h2>
                <h2>in progress</h2>
            </span>
        </div>
        <div class="container5">
            <h1 class="title1">Let's activate your account</h1>
            <h2 class="a1">The application is fast,and only take about 5 minutes</h2>

            <div class="a2">
                <h3 class="a3">First Name*</h3>
                <h3 class="a3">Last Name*</h3>
            </div>

            <div class="a2">
                <h4 class="a4">Nombre</h4>
                <h4 class="a4">Apellido</h4>
            </div>

            <div class="a2">
                <h5 class="a3">Email*</h5>
                <h5 class="a3">Phone*</h5>
            </div>
                
            <div class="a2">
                <h6 class="a4">email@domain.com</h6>
                <h6 class="a4"><img :src="imgsrc" />  +886 | 3455 4546 567</h6>
            </div>
        </div>
    </div>
    <br>
    <div class="container6">
        <button class="b t f">Save and finish later</button>
        <button class="red f">Next Step-></button>
    </div>

</template>

<script>
import ContainerComponent from './components/container.vue';
import ContainerComponent2 from './components/container2.vue';
export default {
  name: 'App',
  components: {
    ContainerComponent,
    ContainerComponent2
  },
  data(){
    return{
        imgsrc: new URL('@/assets/ROC.png', import.meta.url).href,
    }
  }
}
</script>

<style>
  body{
    background: linear-gradient(45deg, pink 40%, white 50%, lightskyblue 60%);
    height: 100vh;
    margin: 0;
  }
#app {
.container3 {
    display: flex;
    border: 1px solid black;
    border-radius: 8px;
    height: 50px;
    justify-content:left;
    align-items: center;
    background-color: white;
    justify-content:space-around;
    margin-left: 10px;
    margin-right: 10px;
}
.wrapper {
    display: flex;
    justify-content: space-between;
    width: 100%;
}
.container4 {
    width: 25%;
    height:550px;
    border: 1px solid black;
    display: flex;
    border-radius: 8px;
    flex-direction: column;
    background-color: white;
    margin-left: 10px;
}
.container5 {
    width: 70%;
    height: 550px;
    border: 1px solid black;
    border-radius: 8px;
    background-color: white;
    margin-right: 10px;
}
.container6{
    display: flex;
    justify-content: end;
    border-radius: 8px;
    margin-left: 10px;
    margin-right: 10px;
}
a {
    text-decoration: none;
    color: #333;
    margin: 0 10px;
}
.b{
    margin-right: 20px;
}
.b3{
    margin-right: 30px;
}
select{
    border: 1px solid black;
    border-radius: 5px;
    background-color: white;
}
.red{
    background-color: red;
    border: 1px;
    border-radius: 5px;
}
.b2{
    margin-right: 500px;
}
.more{
    border: transparent;
}
.btn-box {
    display:inline-block;
    vertical-align:middle;
    width: 40px;
    height: 20px;
    border-radius:100px;
    background-color: #ccc;
    box-shadow: 0px 3px 0px rgba(0,0,0,.13) inset;
}
.btn-box .btn {
    display:inline-block;
    width: 20px;
    height: 20px;
    border-radius:50%;
    background-color: #fff;
    margin-left: 0;/*動畫從ml為0開始*/
    transition: .5s;
    box-shadow:1px 2px 5px rgba(0,0,0,.3);
}
.checkbox {
    position:absolute;
    opacity:0;
}           
.checkbox:checked + .btn-box {
background-color: #8f8;
}
.checkbox:checked + .btn-box .btn {
    margin-left: 20px;
}
.j{
    justify-content: end;
}
.b4{
    margin-right: 120px;
}
.b5{
    margin-right: auto;
}
img{
    background-color: white;
}
.t{
    background-color: transparent;
    border: transparent;
}
.f{
    font-size: 20px;    
}

.title{
    text-align: left;
    color: blue;
    font-weight: bold;
    font-size:20px;
    margin-top:25px;
    margin-left:20px;
    line-height: 0.2;
}

.c1{
    margin-left:120px;
    color: rgb(216, 209, 209);
    font-size:10px;
    line-height: 0.3;
}

.c2{
    margin-top:35px;
}

.title1{
    text-align: left;
    color: blue;
    font-weight: bold;
    font-size:30px;
    margin-top:35px;
    margin-left:20px;
    line-height: 0.2;
}

.a1{
    text-align: left;
    color: rgb(216, 209, 209);
    font-size:10px;
    margin-left:20px;
}


.a2{
    display: flex;
}

.a3{
    justify-content: last baseline;
    text-align: left;
    font-size:20px;
    color: blue;
    margin-top:30px;
    margin-left:20px;
    width: 47%;
}


.a4{
    justify-content: last baseline;
    border: 1px solid rgb(101, 224, 240);
    width: 47%;
    color: rgb(216, 209, 209);
    font-size:15px;
    margin-left:20px;
    margin-top:20px;
    line-height: 2;

}
}
</style>
