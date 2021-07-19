<template>
    <div class="full-flex">
        <div class="left-flex">
        </div>
        <div class="right-flex">       
            <div class="text-box">
            <h1>A borászat</h1>
            <p>
                Mád, mint Tokaj-Hegyalja egyik jelentős történelmi települése, a borvidék meghatározó szőlőterületeivel rendelkezik. E területek változatos vulkanikus talaja, ideális fekvése és egyedi mikroklímája révén magas minőségű, izgalmas borok megszületésének adnak lehetőséget. A borok létrejöttének a szőlőterület, a szőlő és az ezeket kezelő, évszázadok alatt csiszolódott emberi tudás mellett, egy fontos eleme még a borászati épület is. Hegyaljára jellemző módon Mádon is e borászatok többségében nem kint a szőlőben, hanem a település történelmi szerkezetében helyezkednek el, beleilleszkedve a település szövetébe, lakó- és különféle középületek szomszédságában. 
            </p>
                <a href="https://julietvictor.hu/a-birtok/#vinery">TOVÁBB</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        name:"SectionTwo",
    }
</script>

<style lang="scss" scoped>
    
    .full-flex{
        z-index: 10;
        flex-wrap: wrap-reverse;
        display:flex;
        margin-top: 10%;
    }
    .left-flex{
        flex:50%;
        height: 615px;
        background-image: url("./house.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
    }
    .right-flex
    {

        flex:50%;
    }
    .text-box{
        padding-top:15%;
        padding-left:15%;
        padding-bottom: 15%;
        width:80%;
        background-color:white;
    }
    h1{
        text-align: left;
        width: fit-content;
        font-size: xx-large;
        font-weight: 700;
        padding-bottom: 1%;
        border-bottom:1px solid black;
    }
    p{
        margin: 0 0 10px;
        font-size: medium;
        line-height: 2;
        color:black;
        font-family: Roboto;
        font-weight: 200;
        text-align: left;
    }
    a{
        font-family: Roboto;
        font-weight: 600;
        text-decoration: none;
        color:darkslateblue;
        float:left;
    }
     a:visited{
        color:darkslateblue;
    }
    a:hover{
        color:yellow;
    }
    @media only screen and (max-width: 1024px) {
        p{
            font-size: small;
        }
    }
        @media only screen and (max-width: 651px) {
            .full-flex{
                margin-top: -10%;
            }
            .right-flex{
                flex:100%;
                justify-content: center;
            }
            .left-flex{
                margin-top: -200px;
                flex:100%;
                background-size: contain;
            }
            .text-box{
                width:100%;
                padding-left:2%;
                padding-right:2%;

            }
            p{
                font-size: small;
                line-height: 1.5;
                text-align: left;
            }
        }

</style>