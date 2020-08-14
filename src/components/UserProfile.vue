<template>
<div class="userprofile">
<h1> {{msg}} </h1>
<ul>
            <li>
                <router-link to="/neworder" exact> New Order </router-link>
       
                <router-link to="/orderhistory" exact> Order History</router-link>
             
            </li>
        </ul>
</div>
</template>

<script>
export default {
    name:'userprofile',
    data: function(){
        return{
            msg:"Dear User, Bloom Gift cards welcomes you",
            up:"userName"
        }
    },
   
}


</script>

<style scoped>

.router-link-active{
    background-color: lightgrey;
    color: red;
}

li{
    display: inline-block;
    margin: 10px;
    padding: 10px;

}

ul{
    list-style-type: none;

}


</style>