<template>
  <div>
    <div class="outer">
      <table class="indexTable" border="1" cellspacing="0">
        <thead>
          <tr>
            <td colspan="13">xx履行监督责任情况</td>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td class="colspan-1">xx名称</td>
            <td colspan="12"></td>
          </tr>
          <tr>
            <td>履责类型</td>
            <td class="colspan-2" colspan="12">①月度履责②意见建议③讲党课④随手监督</td>
          </tr>
          <tr>
            <td>履责情况</td>
            <td colspan="12"></td>
          </tr>
          <tr rowspan="3">
            <td>监督执纪情况（按月）</td>
            <td colspan="2">廉政谈话数</td>
            <td colspan="2">支部监督信息员报送数</td>
            <td colspan="2">信访处理数</td>
            <td colspan="2">问题线索处置数</td>
            <td colspan="2">立案审查数</td>
            <td colspan="2">运用四种形态数</td>
          </tr>
          <tr>
            <td></td>
            <td>新增</td>
            <td>累计</td>
            <td>新增</td>
            <td>累计</td>
            <td>新增</td>
            <td>累计</td>
            <td>新增</td>
            <td>累计</td>
            <td>新增</td>
            <td>累计</td>
            <td>新增</td>
            <td>累计</td>
          </tr>
          <tr class="row-6">
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
          </tr>
        </tbody>
      </table>
    </div>
    <a href="./second.html">go second tabble</a>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  @import './assets/css/reset.scss';
  .outer{   
    margin: 50px auto;
    .indexTable{
      border: 1px solid black;
      width: px2rem(630);
      text-align: center;
      tr{
        td{
          border: 1px solid black;
          font-size: 16px;
        }
        .colspan-1{
          width: px2rem(116);
        }
        .colspan-2{
          text-align: left;
        }
      }
      thead{
        font-size: 18px;
        font-weight: 700;
        height: px2rem(30); 
      }
      tbody{
        .row-6{
          height: px2rem(52);
        }
      }
    }
  }
</style>