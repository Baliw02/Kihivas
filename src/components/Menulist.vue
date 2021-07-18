<template>
<div class="menu-items">  
    
    <ul>
        <li><img src="./logo.png" alt=""></li>
        <li ><a herf="#">NYITÓLAP</a></li>
        <li class="active"><a herf="#">A BIRTOK</a></li>
        <li ><a herf="#">WEBSHOP</a></li>
        <li ><a herf="#">ÉTTERMEK</a></li>
        <li ><a herf="#">BORKOSTOLÓ</a></li>
        <li ><a herf="#">HIREK</a></li>
        <li ><a herf="#">KAPCSOLAT</a></li>
        <li ><button id="cart"><i class="fa fa-cart-plus" aria-hidden="true"></i></button></li>
        <li ><button id="eng" v-on:click='switchingLang()' class="langs">ENG</button></li>
        <li ><button id="hun" v-on:click='switchingLang()' class="langs act">HUN</button></li>
    </ul>
    
</div>
</template>

<script>
    export default{
        methods:{
            switchingLang(){
                var btn_eng = document.getElementById("eng");
                var btn_hun = document.getElementById("hun");
                btn_eng.classList.toggle("act");

                if(btn_eng.className == "langs act"){
                    btn_hun.classList.remove("act");
                }
                if(btn_eng.className != "langs act"){
                    btn_hun.classList.toggle("act");
                }
            }
        }
    }
</script>
<style lang="scss" scoped>

$sec: rgba(72, 61, 139, 100%);
$prim: white;

img{
    margin-left: 0;
    width:90px;
}

.menu-items{
    padding-top: 1%;
    width: 100%;
}
ul{
    margin-bottom: 0;
    padding-left: 0;
    text-align: center;
}
li {
    margin-inline: 0.8%;
    cursor: pointer;
    font-family: Roboto;
    font-weight: 600;
    width: fit-content;
    font-size: medium;
    display:inline;
    color:$prim;
    transition: all .3s linear;
    
}
.active{
    color: $sec;
}
#cart{
    background-color: $sec;
    border-radius: 10%;
    width:60px;
    transition: all .2s linear;

}
#cart:hover{
    color:$sec;
    background-color: $prim;
}
button{
    border-top: 1px solid black;
    margin-left: 2%;
    width: fit-content;
    font-size: 20px;
    text-align: center;
    border:none;
    background-color: inherit;
    color:$prim;
}
.langs{
    margin-inline: -0.5%;
}
.act{
    border-top:1px solid $sec;
    transition: all .2s linear;
}
li:hover{
    color:$sec;
}


</style>

<style lang="scss">
$sec: rgba(72, 61, 139, 100%);
$prim: white;

</style>
