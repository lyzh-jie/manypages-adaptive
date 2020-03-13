<template>
    <div id="outer">
        <table class="table2" border="1" cellspacing="0">
            <thead>
                <tr>
                    <td colspan="6">xxx片组履行监督责任情况</td>
                </tr>
            </thead>
            <tbody ref="tbo">
                <tr>
                    <td class="col_1">xx名称</td>
                    <td colspan="5"></td>
                </tr>
                <tr>
                    <td class="col_1">履责类型</td>
                    <td colspan="5" class="fontLeft">①周两入企②月度履责③随手简督</td>
                </tr>
                <tr>
                    <td class="col_1">履责情况</td>
                    <td colspan="5"></td>
                </tr>
                <tr>
                   <td rowspan="100">
                       <p>随手简督</p>
                       <p>发现问题</p>
                   </td>
                   <td>序号</td> 
                   <td>问题对象（单位/个人）</td>
                   <td>问题表现</td>
                   <td>整改落实</td>
                   <td>关联指标</td>
                </tr>
                <tr v-for="(item,index) in list" :key="index">
                    <td>{{item.sequenceNumber}}</td>
                    <td>{{item.questionObject}}</td>
                    <td>{{item.quesetionManifestation}}</td>
                    <td>{{item.zhenggailuoshi}}</td>
                    <td>{{item.guanlianzhibiao}}</td>
                </tr>
            </tbody>
        </table>
        <button @click="addRow">添加一行</button>
        <a href="./index.html">go index page</a>
    </div>
</template>

<script>
// const row_str11 = '<tr><td>test</td><td>test</td><td>test</td><td>test</td><td>test</td></tr>';

export default {
    data(){
        return {
            list:[{sequenceNumber:'',questionObject:'',quesetionManifestation:'',zhenggailuoshi:'',guanlianzhibiao:''}]
        }
    },
    methods:{
        addRow:function(){
            console.log(this.$refs.tbo.rows[4]);
            console.log(this.$refs.tbo.rows)
            this.list.push(this.list[0]);            
        }
    }

}
</script>

<style lang='scss' scoped>
    *{
        margin: 0;
        padding: 0;
    }
    @function px2rem($px){
        @return $px/75 + rem;
    }
    #outer{
        .table2{
            margin: 0 auto;
            width: px2rem(626);
            text-align: center;
            thead{
                tr{
                    td{
                        font-size: 17px;
                        font-weight: 700;
                        height: px2rem(26);
                    }
                }
            }
            tbody{
                font-size: 16px;
                tr{
                    .col_1{
                        width: px2rem(117);
                    }
                    td{
                        height: px2rem(30);
                        width: px2rem(103);
                    }
                    .fontLeft{
                        text-align: left;
                    }
                }
            }
        }
    }
</style>