<template>
    <img class="logo" src="./assets/resfo.png">
    <h3>Sign Up</h3>
    <div class="register">
        <input type="text" v-model="name"  placeholder="Enter Name"/>
        <input type="text" v-model="email" placeholder="Enter email"/>
        <input type="password" v-model="password" placeholder="Enter Password"/>
        <button  v-on:click="signUp">Sign Up</button> 
    </div>
</template>
<script>
export default{
    name:'SignUp',
data(){
    return{
        name:'',
        email:'',
        password:''
    }
},
methods:{
    signUp(){
        console.warn("signUp",this.name,this.email,this.password)
    }
}
}
</script>
<style>
.logo{
    width:100px;
}
.register input{
    width:300px;
    height:40px;
    padding-left:20px;
    display:block;
    margin-bottom:30px;
    margin-left:auto;
    margin-right:auto;
    border:1px solid blueviolet;
}
.register button{
    width: 320px;
    height:40px;
    border:1px solid skyblue;
    color:#fff;
    background-color: rgb(14, 113, 179);
    cursor:pointer;
}
</style>
