<template>
    <div class="stop_watches">
        <StopWatch></StopWatch>
        <AddStopWatch></AddStopWatch>
    </div>
</template>

<script>
import StopWatch from "@/components/StopWatch.vue"
import AddStopWatch from "@/components/AddStopWatch.vue"

    export default{
        components:{
            StopWatch, AddStopWatch
        },
    }
</script>

<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    .stop_watches{
        display: flex;
        width: 100%;
        justify-content: space-around;
        align-items: center;
        margin-top: 72px;
    }
    body{
        background-color: #353638;
    }
</style>