<template>
    <div class="full">
        <div class="listing">
            <ul>
                <li><button v-on:click="component='Betsek'">BETSEK</button></li>
                <li><button v-on:click="component='Holdvolgy'">HOLDVÖLGY</button></li>
                <li><button v-on:click="component='Kiraly'">KIRÁLY</button></li>
                <li><button v-on:click="component='Bomboly'">BOMBOLY</button></li>
                <li><button v-on:click="component='Szent'">SZENT-TAMÁS</button></li>
                <li><button v-on:click="component='Veres'">VERES</button></li>
                <li><button v-on:click="component='Uragya'">ÚRÁGYA</button></li>           
            </ul>
        </div>
    <component v-bind:is="component"></component> 

    </div>
</template>

<script>
import Betsek from './GalleryComponents/Betsek'
import Holdvolgy from './GalleryComponents/Holdvolgy'
import Kiraly from './GalleryComponents/Kiraly'
import Bomboly from './GalleryComponents/Bomboly'
import Szent from './GalleryComponents/Szent'
import Veres from './GalleryComponents/Veres'
import Uragya from './GalleryComponents/Uragya'


export default{
    name:'Chooser',
        components:{
        Betsek,
        Holdvolgy,
        Kiraly,
        Bomboly,
        Szent,
        Veres,
        Uragya,
        
        },
        data(){
            return{
                component:'Betsek',
            }
        },


}
</script>
<style lang="scss" scoped>
$sec: rgba(72, 61, 139, 100%);
$prim: white;
.full{
    text-align: center;
    justify-content: center;
}
.listing{
    display: flex;
    justify-content: center;
}
ul{
    justify-content: center;
    text-align: center;
    width: 95%;
    border-bottom: 1px solid black;
    padding-bottom: 1%;
}
li{
    display: inline;
}
button{
    font-family: Roboto;
    font-weight: 300;
    transition: all .3s linear;
    color:$sec;
    border:none;
    background-color:inherit;
    padding:10px 10px;
    margin-inline-end: 1%;
    border:1px solid transparent;
}
button:hover{
    color:$sec;
    border:1px solid $sec;
}
@media only screen and (max-width: 817px) {
    .full{
        margin-top: -20%;
    }
    .listing{
        width: 80%;
        text-align: center;
        justify-content: center;
        margin-left:auto;
        margin-right: auto;
    }
    ul{
        padding-top:20px;
        padding-bottom: 20px;
        border-radius: 15px;
        background-color: $sec;
        padding-left:0;
        width: 100%;
        border-bottom: none;
    }
    li{
        padding-top: 1%;
        display: block;
    }
    button{
        color:$sec;
        background-color: $prim;
        border-radius: 15px;
        text-align: left;
        display:block;
        margin-inline-end: 0;
        width:40%;
        margin-left:auto;
        margin-right:auto;
    }
    button:hover{
        color:$prim;
        background-color: black;
    }
}
@media only screen and (max-width: 651px) {
        button{
            width:70%;
        }
        li{
            padding-top:3%;
        }
}
</style>