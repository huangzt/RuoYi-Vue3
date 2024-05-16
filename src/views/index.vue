<template>
  <div class="app-container home">
    <el-row :gutter="20">
      <el-col :sm="24" :lg="12" style="padding-left: 20px">
        <h2>后台管理框架</h2>
        <h4>内置功能</h4>
        <ul>
          <li>用户管理：用户是系统操作者，该功能主要完成系统用户配置。</li>
          <li>部门管理：配置系统组织机构（公司、部门、小组），树结构展现支持数据权限。</li>
          <li>岗位管理：配置系统用户所属担任职务。</li>
          <li>菜单管理：配置系统菜单，操作权限，按钮权限标识等。</li>
          <li>角色管理：角色菜单权限分配、设置角色按机构进行数据范围权限划分。</li>
          <li>字典管理：对系统中经常使用的一些较为固定的数据进行维护。</li>
          <li>参数管理：对系统动态配置常用参数。</li>
          <li>通知公告：系统通知公告信息发布维护。</li>
          <li>操作日志：系统正常操作日志记录和查询；系统异常信息日志记录和查询。</li>
          <li>登录日志：系统登录日志记录查询包含登录异常。</li>
          <li>在线用户：当前系统中活跃用户状态监控。</li>
          <li>定时任务：在线（添加、修改、删除)任务调度包含执行结果日志。</li>
          <li>代码生成：前后端代码的生成（java、html、xml、sql）支持CRUD下载 。</li>
          <li>系统接口：根据业务代码自动生成相关的api接口文档。</li>
          <li>服务监控：监视当前系统CPU、内存、磁盘、堆栈等相关信息。</li>
          <li>缓存监控：对系统的缓存信息查询，命令统计等。</li>
          <li>在线构建器：拖动表单元素生成相应的HTML代码。</li>
          <li>连接池监视：监视当前系统数据库连接池状态，可进行分析SQL找出系统性能瓶颈。</li>
        </ul>
        <p>
          <b>当前版本:</b> <span>v{{ version }}</span>
        </p>
      </el-col>

      <el-col :sm="24" :lg="12" style="padding-left: 50px">
        <el-row>
          <el-col :span="12">
            <h2>技术选型</h2>
          </el-col>
        </el-row>
        <el-row>
          <el-col :span="6">
            <h4>后端技术</h4>
            <ul>
              <li>SpringBoot</li>
              <li>Spring Security</li>
              <li>JWT</li>
              <li>MyBatis</li>
              <li>Druid</li>
              <li>Fastjson</li>
              <li>...</li>
            </ul>
          </el-col>
          <el-col :span="6">
            <h4>前端技术</h4>
            <ul>
              <li>Vue</li>
              <li>Vuex</li>
              <li>Element-ui</li>
              <li>Axios</li>
              <li>Sass</li>
              <li>Quill</li>
              <li>...</li>
            </ul>
          </el-col>
        </el-row>
      </el-col>
    </el-row>
  </div>
</template>

<script setup name="Index">
const version = ref('3.8.7')

function goTarget(url) {
  window.open(url, '__blank')
}
</script>

<style scoped lang="scss">
.home {
  blockquote {
    padding: 10px 20px;
    margin: 0 0 20px;
    font-size: 17.5px;
    border-left: 5px solid #eee;
  }
  hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid #eee;
  }
  .col-item {
    margin-bottom: 20px;
  }

  ul {
    padding: 0;
    margin: 0;
  }

  font-family: "open sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  color: #676a6c;
  overflow-x: hidden;

  ul {
    list-style-type: none;
  }

  h4 {
    margin-top: 0px;
  }

  h2 {
    margin-top: 10px;
    font-size: 26px;
    font-weight: 100;
  }

  p {
    margin-top: 10px;

    b {
      font-weight: 700;
    }
  }

  .update-log {
    ol {
      display: block;
      list-style-type: decimal;
      margin-block-start: 1em;
      margin-block-end: 1em;
      margin-inline-start: 0;
      margin-inline-end: 0;
      padding-inline-start: 40px;
    }
  }
}
</style>

