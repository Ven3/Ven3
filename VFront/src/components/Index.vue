<template>
  <div id="task">
    <label >添加用户</label>
    <form role="form">
      <div class="form-group text-left">
        <label for="username">用户名:</label>
        <input type="text" id="username" class="form-control">
      </div>
      <div class="form-group text-left">
        <label for="age">年龄</label>
        <input type="text" id="age" class="form-control">
      </div>
      <div class="form-group text-left">
        <button class="btn btn-primary">登录</button>
        <button class="btn btn-danger">重置</button>
      </div>
    </form>
    <hr>
    <table class="table table-bordered table-hover" role="table">
      <caption class="h2 text-info">用户信息表</caption>
      <tr class="text-center h4">
        <th>序号</th>
        <th>名字</th>
        <th>年龄</th>
        <th>操作</th>
      </tr>
      <tr >
        <td>1</td>
        <td>andy</td>
        <td>25</td>
        <td>
          <button class="btn btn-sm btn-info">修改</button>
          <button class="btn btn-sm btn-danger">删除</button>
        </td>
      </tr>
      <tr >
        <td>1</td>
        <td>andy</td>
        <td>25</td>
        <td>
          <button class="btn btn-sm btn-info">修改</button>
          <button class="btn btn-sm btn-danger">删除</button>
        </td>
      </tr>
      <tr >
        <td>1</td>
        <td>andy</td>
        <td>25</td>
        <td>
          <button class="btn btn-sm btn-info">修改</button>
          <button class="btn btn-sm btn-danger">删除</button>
        </td>
      </tr>
      <tr>
        <td colspan="4" class="text-right">
          <button class="btn btn-danger btn-sm" data-toggle="modal" data-target="#msgbox">删除全部</button>
          <button class="btn btn-success" data-toggle="modal" data-target="#msgbox">弹框</button>
        </td>
      </tr>
      <tr>
        <td colspan="4" class="text-center text-muted">
          <p>暂无数据...</p>
        </td>
      </tr>
    </table>

    <div role="dialog" class="modal fade" id="msgbox">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <button class="close" data-dismis="msgbox"><span>&times;</span></button>
            <div class="modal-title">是否删除??</div>
          </div>
          <div class="modal-body">
            <button class="btn btn-primary btn-sm">取消</button>
            <button class="btn btn-danger btn-sm">确定</button>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
    export default {
        name: "Index"
    }
</script>

<style scoped>

</style>
