<template>
  <div class="segment" style="padding:0;">
    <table class="table table-9">
      <tr>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/1.png" alt="pic">
            <p>收款统计</p>
          </div>
        </td>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/2.png" alt="pic">
            <p>菜品销售</p>
          </div>
        </td>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/3.png" alt="pic">
            <p>优免统计</p>
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/4.png" alt="pic">
            <p>退菜统计</p>
          </div>
        </td>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/5.png" alt="pic">
            <p>赠菜统计</p>
          </div>
        </td>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/6.png" alt="pic">
            <p>沽清统计</p>
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <div class="table-9-cell">
            <img src="@/assets/7.png" alt="pic">
            <p>桌型利用率</p>
          </div>
        </td>
        <td></td>
        <td></td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
  .table-9 tr td {
    width: 30%;
    position: relative;
    padding: 23px 0;
  }
  .table-9 tr td::after {
    content: '';
    height: 200%;
    width: 200%;
    position: absolute;
    top: 0;
    left: 0;
    border-bottom: 1px solid #e5e5e5;
    border-right: 1px solid #e5e5e5;
    transform: scale(.5);
    -webkit-transform: scale(.5);
    transform-origin: 0 0;
    -webkit-transform: 0 0;
  }
  /* 把td为偶数的右边框显示出来 */
  .table-9 tr td:nth-child(even)::after {
    border-right: 1px solid #eeeeee;
  }
  /* 把td为3的倍数的右边框去掉 */
  .table-9 tr td:nth-child(3n+3)::after {
    border-right: none;
  }
  .table-9-cell {
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
  }
  .table-9-cell img {
    width: 50px;
  }
  .table-9-cell p {
    color: #525252;
  }
</style>
