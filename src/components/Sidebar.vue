<template>
<div class="side">
    <img src="./logo.png">
    <b-button id="toggler" v-b-toggle.sidebar-1 ><i class="fa fa-bars" aria-hidden="true"></i></b-button>
        <b-sidebar backdrop id="sidebar-1" backdrop-variant="dark" bg-variant="dark" text-variant="light" shadow>
        <div class="px-3 py-2">
            <h1>Juliet Victor</h1>
            <ul>
                <li ><a herf="#">NYITÓLAP</a></li>
                <li class="active"><a herf="#">A BIRTOK</a></li>
                <li ><a herf="#">WEBSHOP</a></li>
                <li ><a herf="#">ÉTTERMEK</a></li>
                <li ><a herf="#">BORKOSTOLÓ</a></li>
                <li ><a herf="#">HIREK</a></li>
                <li ><a herf="#">KAPCSOLAT</a></li>
            </ul>
        </div>
    </b-sidebar>
    <div class="others">
        <button id="cart"><i class="fa fa-cart-plus" aria-hidden="true"></i></button>
        <button id="eng" v-on:click='switchingLang()' class="langs">ENG</button>
        <button id="hun" v-on:click='switchingLang()' class="langs act">HUN</button>
    </div>
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

.others{
    text-align: right;
}
img{
    margin-top: -0.5%;
    padding: 0;
    float:left;
    width:12%;
}
button{
    border:none;
}
#cart{
    background-color: rgba(72, 61, 139, 100%);
    border-radius: 10%;
    width:60px;
    color:white;
}
#toggler{
    background-color: black;
    width:fit-content;
    z-index: 10;
    float:right;
    margin-bottom: 0;
    margin-top: -5px;

}
.langs{
    font-size: small;
    background-color: black;
    color:white;
    margin-inline: 1%;
}
.act{
border-top:1px solid $sec;
transition: all .2s linear;
}
ul{
    padding-left: 0;
    margin-left: 0;
    list-style: none;
    text-align: left;
}
li{
    line-height: 3;
    font-family: Roboto;
    font-weight: 500;
    color:white;
    font-size: medium;
}
h1{
    font-size: xx-large;
    font-weight: 500;
    text-align: left;
    padding-left:0;
    border-bottom: 1px solid white;
}
</style>

