<template>
    <div class="Pos">
        <le-row>
            <el-col :span='7' class="pos-order" id='order-list'>
                我是订单栏
            </el-col>
            <el-col>
                我是产品栏
            </el-col>
        </le-row>
    </div>
</template>

<script>
export default {
    name:'Pos',
    data(){
        return{

        }
    },
    mounted:function(){
        var orderHeight=document.body.clientHeight;
        console.log(orderHeight)
        document.getElementById('order-list').style.height=orderHeight+'px'
    }
}
</script scoped>

<style>
.pos-order{
    background-color: #f9fafc;
    border-right: 1px solid #c0ccda;

}
</style>
