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
                <img src="./Images/veres01.jpg">
            </slide>
            <slide>
                <img src="./Images/veres02-1200x800.jpg">
            </slide>
            <slide>
                <img src="./Images/veres03.jpg">
            </slide>
            <slide>
                <img src="./Images/veres04.jpg">
            </slide>         
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Veres</strong></h1>
    <p>
        A magas talajminőségű Veres dűlőben 1,4 hektáron 2,6 m x 1 m-es térállású szőlő ültetvénnyel rendelkezünk. Tőkéink 35 évesek - furmint és 
        hárslevelű fajtaösszetétellel dolgozunk. A Veres dűlőt 100%-ban az édes szamorodni és aszú borok alapboraiba használjuk ezért a madarak dézsmálása 
        ellen hálózzuk a területet, így óvjuk az egyedülálló termést. A szüretet novemberben kezdjük az ültetvényen, amelynek termése 
        kimagaslóan botritizálódik, aszúsodik a tufának és a vörösagyag vízmegtartó képességének köszönhetően.
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Veres"
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