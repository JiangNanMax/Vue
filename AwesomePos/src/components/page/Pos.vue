<template>
    <div class="pos">
        <div class="">
            <el-row>
                <el-col :span='6' class="pos-order" id="order-list">
                    <el-tabs>
                        <el-tab-pane label="点餐">
                            <el-table :data="tableData" border show-summary style="width: 100%">
                                <el-table-column prop="goodsName" label="商品" width="100"></el-table-column>
                                <el-table-column prop="count" label="数量" width="50"></el-table-column>
                                <el-table-column prop="price" label="金额" width="50"></el-table-column>
                                <el-table-column prop="" label="操作" width="100" fixed="right">
                                    <template scope="scope">
                                        <el-button type="text" size="small">删除</el-button>
                                        <el-button type="text" size="small">增加</el-button>
                                    </template>
                                </el-table-column>
                            </el-table>
                            <div class="">
                                <el-button>结算</el-button>
                                <el-button>挂单</el-button>
                                <el-button>删除</el-button>
                            </div>
                        </el-tab-pane>

                        <el-tab-pane label="挂单">

                        </el-tab-pane>

                        <el-tab-pane label="外卖">

                        </el-tab-pane>
                    </el-tabs>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
export default {
  name: 'pos',
  data(){
      return{
          tableData: [{
          goodsName: '可口可乐',
          price: 8,
          count:1
        }, {
          goodsName: '香辣鸡腿堡',
          price: 15,
          count:1
        }, {
          goodsName: '薯条',
          price: 8,
          count:1
        }, {
          goodsName: '甜筒',
          price: 8,
          count:1
        }]
      }
  },
  mounted: function(){
      var orderHeight = document.body.clientHeight;
      console.log(orderHeight);
      document.getElementById("order-list").style.height=orderHeight+'px';//!!!
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pos-order {
    background-color: #F9FAFC;
    border-right: 1px solid #C0CCDA;
    height: 100%;
}
</style>
