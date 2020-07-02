<template>
    <div class="out1" :style="{...DoHe}">
    <h1>{{day}}</h1>
    <h2>{{time}}</h2>
    <h3>{{name}}</h3>
    <p>倒计时:
    <span>{{min}}</span>
    <input type="button"/>
    </p>
    <!-- <hr style="height:10%"/> -->
    </div>
</template>>
<script>
export default {
    data() {
        return {
            day:'白天',
            name:'希图斯',
            time:'00:21:00',
            min:'21',
        }
    },
    props:{
        he:{
            type:Number,
            default:1,
        },
    },
    computed:{
        DoHe(){
            return {
                'height':this.he+'rem',
            }
        }
    }
}
</script>>
<style scoped lang="scss">
@each $out in 1{
    .out#{$out}{
        //width:100%;
        margin: {
            top:5px;
            bottom: 5px;
            left:10px;
            right:10px;
        };
        background-color: #ee7b6e;
        border-radius: 0.5rem;
        display: flex;
    }
}
</style>