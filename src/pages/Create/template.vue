<template>
   <div id="create">
    <h1>创建文章</h1>
    <h3>文章标题</h3>
    <el-input v-model="title" placeholder="请输入内容">></el-input>
    <p class="msg">限30个字</p>
    <h3>内容简介</h3>
    <el-input v-model="description" type="textarea" :autosize="{ minRows: 2, maxRows: 6}" rows=3 placeholder="请输入内容"></el-input>
    <p class="msg">限30个字</p>
    <h3>文章内容</h3>
    <el-input v-model="content" type="textarea" rows=20 :autosize="{ minRows: 4, maxRows: 30}" placeholder="请输入内容"></el-input>
    <p class="msg">限60个字</p>
    <p>
        <label>是否展示到首页</label>
        <el-switch v-model="atIndex" active-color="#13ce66" inactive-color="#ff4949"></el-switch>
    </p>
    <el-button @click="onCreate" class="btt">立即创建</el-button>
  </div>
</template>

<script src="./template.js"></script>

<style lang="less" src="./template.less">
 
</style>