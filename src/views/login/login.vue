<template>
  <div class="login-page">
    <div class="header">
      <span class="arrow-left">
        <i class="el-icon-back"></i>
      </span>
      <div class="header-desc">
        <span>网易邮箱账号登录</span>
      </div>
      <!-- <span class="arrow-right">
                <i class="el-icon-right"></i>
            </span> -->
    </div>
    <div class="main">
      <el-form>
        <el-form-item>
          <el-input placeholder="请输入邮箱账号"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input placeholder="密码"></el-input>
        </el-form-item>
      </el-form>
    </div>
    <div class="footer">
      <el-button type="success">登录</el-button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Login",
  components: {},
  data() {
    return {};
  },

  mounted() {
    this.init();
  },
  methods: {
    init() {}
  }
};
</script>

<style lang="less" scoped>
.login-page {
  .main {
    background-color: #fff;
    padding: 0.5rem;
    margin: 0.5rem 0 2rem;
    /deep/.el-input__inner {
      border: 0;
      border-bottom: 1px solid #dcdfe6;
      border-radius: 0;
    }
  }
  .footer {
    padding: 0 0.5rem;
    .el-button {
      width: 100%;
    }
  }
}
.header {
  height: 1.95rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 0.5rem;
  .arrow-left,
  .arrow-right {
    flex: 1;
  }
  .arrow-left {
    text-align: left;
  }
  .arrow-right {
    text-align: right;
  }
  .header-desc {
    flex: 4;
  }
}
</style>
