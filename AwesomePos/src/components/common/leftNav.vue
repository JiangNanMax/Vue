<template>
    <div class="leftnav">
        <ul>
            <li>
                <i class="icon iconfont icon-goumai"></i>
                <div class="">收银</div>
            </li>
            <li>
                <i class="icon iconfont icon-dianpu"></i>
                <div class="">店铺</div>
            </li>
            <li>
                <i class="icon iconfont icon-hanbao"></i>
                <div class="">商品</div>
            </li>
            <li>
                <i class="icon iconfont icon-huiyuanqia"></i>
                <div class="">会员</div>
            </li>
            <li>
                <i class="icon iconfont icon-37"></i>
                <div class="">统计</div>
            </li>
            <li>
                <i class="icon iconfont icon-gongnengjianyi"></i>
                <div class="">设置</div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'leftNav',
    data(){
        return {

        }
    }
}
</script>

<style>
    .leftnav{
        color: #fff;
        font-size: 10px;
        height: 100%;
        background-color: #1D8CE0;
        float: left;
        width: 5%;
    }
    .iconfont{
        font-size: 25px;
    }
    .leftnav ul{
        padding: 0px;
        margin: 0px;
    }
    .leftnav li{
        list-style: none;
        text-align: center;
        border-bottom: 1px solid #20a0ff;
        padding: 10px;
    }
</style>
