# generate-resume-pdf

> 使用Vue编写可以个性化样式的简历

## html2pdf.js

**github:** [html2pdf.js](https://github.com/eKoopmans/html2pdf)

### 遇到的问题

- vue-cli init webpack [project-name]时出现安装依赖失败的情况
- li 标签默认的黑色圆点渲染失败
- 导出 pdf 时 margin 值的设置会导致一些视图的样式错乱

### 解决方案

- npm cache clean --force 之后,npm i -g npm 重新安装
- 使用标签 before css 属性设置替代符号 ">"
- 根据错乱情况，调整样式的比例 
