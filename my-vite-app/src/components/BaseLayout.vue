<template>
  <div class="app-container">
    <!-- 侧边栏 -->
    <aside class="sidebar">
      <div class="logo">系统名称</div>
      <nav class="sidebar-nav">
        <ul>
          <li>仪表盘</li>
          <li>用户管理</li>
          <li>产品管理</li>
          <li>订单管理</li>
          <li>系统设置</li>
        </ul>
      </nav>
    </aside>
    
    <!-- 主内容区域 -->
    <div class="main-container">
      <header class="top-nav">
        <div class="breadcrumbs">首页 / 仪表盘</div>
        <div class="user-info">管理员</div>
      </header>
      
      <main class="page-content">
        <h1>仪表盘</h1>
        <div class="content-area">
          <p>主内容区域</p>
        </div>
      </main>
    </div>
  </div>
</template>

<script setup>
// 无额外逻辑
</script>

<style scoped>

/* 1. 最外层容器 - 水平布局 */
.app-container {
  display: flex;
  min-height: 100vh; /* 占满整个视口高度 */
}

/* 2. 侧边栏 - 固定宽度 */
.sidebar {
  width: 200px;
  background-color: #2c3e50;
  color: white;
}

.logo {
  padding: 16px;
  font-weight: bold;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.sidebar-nav ul {
  list-style: none;
}

.sidebar-nav li {
  padding: 12px 16px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

/* 3. 主内容容器 - 占满剩余空间 */
.main-container {
  flex: 1;
  display: flex;
  flex-direction: column;
}

/* 4. 顶部导航栏 */
.top-nav {
  height: 60px;
  background-color: #f8f9fa;
  border-bottom: 1px solid #e0e0e0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
}

/* 5. 页面内容区 */
.page-content {
  flex: 1;
  padding: 20px;
  background-color: #f5f7fa;
  overflow-y: auto;
}

.content-area {
  background-color: white;
  padding: 20px;
  min-height: 300px;
}
</style>