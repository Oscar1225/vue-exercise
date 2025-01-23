<template>
    <div>
        <ContainerComponent />
    </div>
    <div>
        <ContainerComponent2/>
    </div>
    <br>
    <div>
        <ContainerComponent3/>
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
import ContainerComponent3 from './components/container3.vue';
export default {
  name: 'App',
  components: {
    ContainerComponent,
    ContainerComponent2,
    ContainerComponent3,
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
