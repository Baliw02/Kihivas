<template>
    <div>
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
                component:'Betsek'
            }
        }
    }
</script>
<style lang="scss" scoped>
     .listing{
        display: flex;
        justify-content: center;
    }
    ul{
        text-align: center;
        width: 95%;
        border-bottom: 1px solid black;
        padding-bottom: 1%;
    }
    li{
        font-family: Roboto;
        font-weight: 200;
        margin-inline: 1%;
        display: inline;
    }
    button{
        
        border:none;
        background-color:inherit;
    }
</style>