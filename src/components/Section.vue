<template>
    <div class="full-flex">
        <div class="left-flex">
            <h1>Történet</h1>
            <p>
            <span><b>Magyarország elsőrangú és kivételes borainak legjava.</b><br></span>
            A Váradi család vaxco birtoka Mádon, az UNESCO világörökség részévé nyilváníitott, történelmi, Tokaji borvidék területén található – 
            egy kivételesen gazdag terroir, amely különféle termőtalajok találkozásából keletkezett. A Juliet Victor sokrétű világa megteremti a 
            tökéletes egyensúlyt történelmi és modern között: nagy múltú terroir és csúcstechnológiát alkalmazó előállítás. A Juliet Victor elegáns, 
            száraz fehér és igazán egyedülálló, édes desszertborokat alkot a bor szerelmeseinek.
            </p>
            <a href="https://julietvictor.hu/a-birtok/#history">TOVÁBB</a>
        </div>
        <div class="right-flex">
        </div>
    </div>
</template>

<script>
    export default{
        name:"Section-One",
    }
</script>

<style scoped>
    .full-flex{
        background-position: center;
        background-image:url("./backsecond.jpg");
        background-size: cover;
        background-attachment: fixed;
        background-repeat: no-repeat;
        margin-top: 20%;
        clear:none;
        width: 100%;
        display: flex;
        padding-bottom: 5%;

    }
    .left-flex{     
        margin-top: -5%;
        margin-left: 10%;
        background-color: black;
        text-align: left;
        width: 100%;
        flex:20%;
        padding:100px 100px;
    }
    .heading{
        width: fit-content;
    }
    span{
        font-size: medium;
        font-style: bold;
    }
    p{
        line-height: 2;
        font-size: small;
        font-family: Roboto;
        font-weight: 200;
        text-align: left;
        color:white;
    }
    h1{
        font-size: xx-large;
        width: fit-content;
        color:white;
        padding-bottom: 5px;
        border-bottom: 2px solid white;
    }

    a{
        font-size: 13px;
        font-family: Roboto;
        font-weight: 700;
        text-decoration: none;
    }
    a:visited{
        color:white;
    }
    a:hover{
        color:yellow;
    }
   
    .right-flex{
        width: 100%;
        flex:50%;
    }
        @media only screen and (max-width: 1054px) {
            .left-flex{
                flex:50%;
            }
        }
        @media only screen and (max-width: 769px) {
            .left-flex{
                flex:80%;
            }
        }
        @media only screen and (max-width: 455px) {
            h1{
                font-size: medium;
            }
            p{
                font-size: smaller;
            }
            .full-flex{
                display:block;
                background-attachment: scroll;
                background-size: 100%;
                background-position: center;
                margin-bottom: 100px;
                margin-top: 100%;
            }
            .left-flex{
                position: relative;
                top:-300px;
                padding:30px 30px;
                margin-left: 0;
                width:100%;            
            }
            .right-flex{
                flex:0;
            }
        }


</style>