<template>
    <div class="main">
        <div class="timer">
            <div class="timer_block">
                <p class="time hour">00</p>
            </div>
            :
            <div class="timer_block">
                <p class="time minute">00</p>
            </div>
            :
            <div class="timer_block">
                <p class="time second">00</p>
            </div>
        </div>
        <div class="buttons">
            <button id="start"></button>
            <button id="stop" hidden></button>
            <button id="reset"></button>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
    .main{
        width: 255px;
        height: 120px;
        background-color: #696969;
        margin: 0px 70px 30px 70px;
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
    .timer{
        display: flex;
        height: 50%;
        justify-content: center;
        align-items: center;
    }
    .timer_block{
        color: black;
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