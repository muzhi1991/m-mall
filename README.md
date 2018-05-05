# 微信小程序-移动端小商城

## 项目说明：

- 基于微信小程序开发的一款移动端小商城
- 基于 weui.wxss、es6 前端技术开发
- 基于 [wx-extend](https://github.com/skyvow/wx-extend) 第三方扩展插件（发送请求、Promise API、表单验证）
- 前台 [m-mall](https://github.com/skyvow/m-mall)
- 后台 [m-mall-admin](https://github.com/skyvow/m-mall-admin)

## 开发环境

1. 推荐使用vscode编写代码，安装下列插件
* minapp: wxml代码提示，参考功能参考[文档](https://qiu8310.github.io/minapp/docs/doc-autocomplete.html)
* 使用typings自动提示api，功能参考[文档](https://qiu8310.github.io/minapp/docs/doc-autocomplete.html)：
  * 在项目根目录下运行`npm install  @minapp/wx`
  * 在入口文件app.js中添加下列内容（我已经添加了，不用加入了）
  * 如果需要更新，在项目根目录下运行`npm update  @minapp/wx`
  
  ```js
  /// <reference path="./node_modules/@minapp/wx/typing/app.d.ts" />
  /// <reference path="./node_modules/@minapp/wx/typing/behavior.d.ts" />
  /// <reference path="./node_modules/@minapp/wx/typing/component.d.ts" />
  /// <reference path="./node_modules/@minapp/wx/typing/page.d.ts" />
  /// <reference path="./node_modules/@minapp/wx/typing/wx.d.ts" />
  ```

* 小程序助手: wxss代码高亮
* vscode weapp api: 提供了js的代码模板，wxXXX即可提示，如wxpage会有page模板，wxrequest会有请求模板
* WeApp Snippets: 提供了wxml程序模板，在wxml中输入wa开头会有，wa-button会有button的模板

> 注意，添加api提示，还可以在项目中添加了jsconfig.json文件和typings目录的api提示配置（复制node_modules/@minapp/wx/typing到项目根目录的typings目录下）。

2. 使用官方小程序工具预览代码，代码保存会自动触发重新编译。其他方案如wept已经不维护，不推荐使用。


## 目录结构：

```
m-mall/
  |-assets/                     # 静态文件
     |- images/                 # 图片
     |- plugins/                # 插件
     |- styles/                 # 样式
     |- ...
  |-etc/                        # 配置文件
     |- config.js
     |- ...
  |-helpers/                    # 帮助文件
     |- HttpResource.js
     |- HttpService.js
     |- ...
  |-pages/                      # 小程序页面相关文件
      |- start
        |- index.js
        |- index.json
        |- index.wxml
        |- index.wxss
      |- ...
  |-app.js                      # 小程序逻辑
  |-app.json                    # 小程序公共设置
  |-app.wxss                    # 小程序公共样式表
  |-...
```

## 项目截图:

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-11.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-12.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-13.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-01.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-02.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-03.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-04.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-05.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-06.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-14.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-07.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-08.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-09.png" width="375px" style="display:inline;">

<img src="https://github.com/skyvow/m-mall/blob/master/assets/images/screenshots/screenshorts-10.png" width="375px" style="display:inline;">

##	贡献

有任何意见或建议都欢迎提 issue

##	License

MIT