<template>
    <div class="main">
        <div class="watches">
            <p class="center">1111:222::333</p> 
        </div>
        <div class="buttons">
            <!-- Start/Stop -->
            <button id="start"></button>

            <button id="stop"></button>
            <!-- Reset -->
            <button id="reset"></button>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .main{
        width: 255px;
        height: 120px;
        background-color: #696969;
    }
    .buttons{
        display: flex;
        justify-content: center;
        align-items: center;
        border-top:2px solid #ffffff;
        height: 50%;
    }
    .watches{
        height: 50%;
        width: 100%;
        justify-content: center;
        align-items: center;
    }
    .center{
        display: flex;
        justify-content: center;
        height: 100%;
        align-items: center;
    }
    /* Custom Buttons */
    #reset{
        width: 20px;
        height: 20px;
        background-color: #ffffff;
        border: 0px;
        margin-left: 48px;
    }
    #start{
        background-color: #696969;
        width: 0;
        height: 0;
        border: transparent;
        border-top: 10px solid transparent;
        border-left: 17px solid #ffffff;
        border-bottom: 10px solid transparent;
    }
    #start:hover{
        border-left: 17px solid #55555f;
    }
    #reset:hover{
        background-color: #55555f;
    }
    #stop{
        background: #9E9E9E;
        height: 20px;
        position: relative;
        border: 0px;
        width: 3px;
        left: 5px;
    }
    #stop:after{
        background: #9E9E9E;
        content: "";
        height: 20px;
        left: 7px;
        top: 0px;
        position: absolute;
        width: 3px;
    }
    #stop:hover{
        background: #ffffff;
    }
    #stop:hover::after{
        background: #ffffff;    
    }
</style>