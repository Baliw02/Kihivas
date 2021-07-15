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
                <img src="./Images/bomboly01.jpg">
            </slide>
            <slide>
                <img src="./Images/bomboly02.jpg">
            </slide>
            <slide>
                <img src="./Images/bomboly03.jpg">
            </slide>
            <slide>
                <img src="./Images/bomboly04.jpg">
            </slide>
            <slide>
                <img src="./Images/bomboly05.jpg">
            </slide>    
            <slide>
                <img src="./Images/bomboly06.jpg">
            </slide>             
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Bomboly</strong></h1>
    <p>
        A délnyugati 
        fekvésű, szépséges Bomboly dűlőben 6 hektár 2,4 m x 1 m-es ültetvény található. A fajta összetételeknek, a 
        vulkanikus talajnak és a tőkék korának köszönhetően az egyik legegyedibb területen találhatjuk magunkat. Mintegy 1,2 
        hektárt 2018-ban újra telepítettünk 100% furmint fajtával - a dűlőben található a legöregebb ültetvényünk, maguk a 102 éves 
        furmint tőkék. A rendkívül meredek, hosszan elnyúló 300 m-es sorok a hegy tetejétől, egészen a völgy aljáig húzódnak, ennek 
        köszönhetően a völgy párája minden évben nagyobb botritizálódást, aszútermést eredményez. Ebből az adottságból következően születhetnek a 
        területről származó száraz, édes szamorodni és aszú boraink.
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Bomboly"
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