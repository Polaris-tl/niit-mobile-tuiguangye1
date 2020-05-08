<template>
    <div>
        <p>{{title1}}</p>
        <p>{{title2}}</p>
    </div>
</template>

<script>
export default {
    name:"SmallHead",
    props:{
        title1:String,
        title2:String
    }
}
</script>

<style lang="less" scoped>
 div{

 }
    p:nth-child(1){
        font-size: 16px;
        font-family: "Microsoft YaHei";
        color: rgb(21, 21, 21);
        font-weight: bold;
        line-height: 1.2;
        position: relative;
        left: 16px;
        &::after{
            content: '';
            width: 4px;
            height: 20px;
            background: #0d87fc;
            position: absolute;
            top: 0;
            bottom:0;
            margin:auto;
            left: -16px;

        }
    }
    p:nth-child(2){
        font-size: 13px;
        font-family: "Microsoft YaHei";
        color: rgb(160, 160, 160);
        line-height: 1.2;
        margin-top: 4px
    }
</style>