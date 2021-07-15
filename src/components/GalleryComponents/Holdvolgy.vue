<template>
<div class="full-flex">
    <div class="left-flex">
        <carousel
            :paginationEnabled="true"
            :paginationActiveColor="'#35254d'"
            :paginationColor="'#000000'"
            :paginationPadding="2"
            :per-page="1"
            :touchDrag="false"
            :centerMode="true"
            :spacePadding="0"
        >
            <slide>
                <img src="./Images/holdvolgy01.jpg">
            </slide>
            <slide>
                <img src="./Images/holdvolgy02.jpg">
            </slide>
            <slide>
                <img src="./Images/holdvolgy03.jpg">
            </slide>
            <slide>
                <img src="./Images/holdvolgy04.jpg">
            </slide>         
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Holdvölgy</strong></h1>
    <p>
        A festői szépségű Holdvölgy dűlőben 3,2 hektáron 2,4 m x 0,9 m-es térállású szőlő található – ezen a helyen több kis parcellából áll össze az ültetvény, 
        ezért különböző korú és a Furmint fajtáján belül is különböző alfajták termesztünk a területen, többek közt a T 85-öset, a madárkást vagy a hólyagosat. 
        Ennek a rendhagyó körülménynek köszönhetően nagyon érdekes a Holdvölgy dűlőhöz köthető ízvilág és komplexitás. A talaj vörösagyag és kvarc tartalmú kőzet keveréke – 
        szőlősorok pedig egy lankás dombon, 300 méter hosszúságban terülnek el. Egyes helyeken 
        hidrokvarcit képződés mutatkozik, amely nagy mértékű hidrotermás vulkáni munkára utal. 
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Holdvolgy"
    }


</script>

<style scoped>
    .VueCarousel-slide{
        position:relative;
    }
    .VueCarousel{
        width:100%;
        display:flex;
}
   
    .full-flex{
        width: 100%;
        display: flex;
        flex-wrap: nowrap;
    }
    .left-flex{
        margin-left:0;
        justify-content: left;
        width:60%;
        flex:60%;
    }
    .right-flex{
        justify-content: center;
        flex:40%;
        width:40%;
        padding-left: 5%;
        padding-right: 10%;
    }
    img{
        max-width:100%;
    }
    p{
        padding-right: 150px;
        font-weight: 300;
        font-size: medium;
        text-align: justify;
        line-height: 2;
    }
    h1{
        color:black;
        font-size: xx-large;
        width: fit-content;
        border-bottom: 1px solid black;
    }
    @media only screen and (max-width: 812px) {
        .full-flex{
            padding: 1%;
            flex-wrap: wrap;
        }
         .left-flex{
            flex:100%;
        }
        .right-flex{
            flex:100%;
            padding-left: 0;
            padding-right: 0;

         }
        p{
                padding-left:5px;
                padding-right: 5px;
        }
        }
        @media only screen and (max-width: 1280px) {
                        p{
                font-size: small;
                padding-left: 5px;
                padding-right: 5px;
            }
        }


</style>