<template>
  <div id="resume">
    <LevelTitle level="2" content="基本信息"/>
    <LabelWithValue label="姓名" value="苑朋飞"/>
    <LabelWithValue label="英文名" value="Peter"/>
    <LabelWithValue label="出生年月" value="1993/02"/>
    <LabelWithValue label="手机号" value="18518981046"/>
    <LabelWithValue label="E-Mail" value="ypf9319@gmail.com" isLink="true"/>
    <LabelWithValue label="github" value="https://github.com/GitHubJiKe" isLink="true"/>
    <LabelWithValue label="毕业院校" value="防灾科技学院"/>
    <LabelWithValue label="专业" value="计算机科学与技术"/>
    <LevelTitle level="2" content="工作经历"/>
    <level-title style="padding:0px 20px;" level="3" content="映客"/>
    <LabelWithValue label="时间" value="2015/11 ~ 2016/04"/>
    <LabelWithValue label="职位" value="Android 实习开发"/>
    <LabelWithValue label="主要职责" value="功能模块开发，代码优化及重构"/>
    <level-title style="padding:0px 20px;" level="3" content="彪洋科技"/>
    <LabelWithValue label="时间" value="2016/04 ~ 至今"/>
    <LabelWithValue label="职位" value="Software Enginner"/>
    <LabelWithValue label="主要职责" value="公司内部产品研发及外包项目研发（前端）"/>
    <div class="detail">
      <level-title level="4" content="工作细节"/>
      <ul>
        <li>使用React、NodeJs技术开发广汽菲克及本公司财务管理系统</li>
        <li>与PO一起进行需求分析，给出客户满意的解决方案</li>
        <li>使用Vue框架承接保时捷公司H5页面，提供实现可配置化解决方案</li>
        <li>与团队一起使用React框架进行保时捷公司售前管理系统的重构</li>
        <li>与PO和院队成员一起需求分析，讨论解决方案，攻克技术难题</li>
        <li>参与敏捷开发流程培训和实践，参与story划分和task拆分过程</li>
        <li>参与代码重构和优化分享</li>
        <li>结对编程，帮助实习生快速成长</li>
      </ul>
    </div>
    <div class="html2pdf__page-break"></div>
    <level-title level="2" content="核心技能"/>
    <div class="detail">
      <level-title level="3" content="基础"/>
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JS</li>
      </ul>
      <level-title level="3" content="框架"/>
      <ul>
        <li>React 及其工具链</li>
        <li>Vue 及其工具链</li>
        <li>小程序 及其工具链</li>
        <li>antd ui</li>
        <li>element ui</li>
        <li>echarts</li>
      </ul>
      <level-title level="3" content="其他"/>
      <ul>
        <li>node</li>
        <li>webpack</li>
        <li>git</li>
      </ul>
    </div>
    <level-title level="2" content="兴趣爱好"/>
    <div class="detail">
      <ul>
        <li>健身</li>
        <li>跑步</li>
        <li>做饭</li>
        <li>电影</li>
      </ul>
    </div>
    <footer class="footer">
      @power by Peter Yuan<br/>
      with Vue & html2pdf.js<br>
      <a href="https://github.com/GitHubJiKe/generate-resume-pdf.git">项目地址</a>
    </footer>
  </div>
</template>

<script>
import LevelTitle from './LevelTitle.vue'
import LabelWithValue from './LabelWithValue.vue'
export default {
  name: 'Index',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    LevelTitle,
    LabelWithValue
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.detail{
  margin-top: 20px;
  padding: 0px 40px;
}
.detail li{
  padding: 3px 0px;
}
.detail li::before{
  content: ">";
  font-weight: bolder;
  margin-right: 5px;
}
.footer{
  margin-top: 100px;
  text-align: center;
  color: gray;
}
</style>
