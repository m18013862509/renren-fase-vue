## 下载运行之后存在的问题：
- 个人在GitHub上下载代码之后，自己在运行的时候会遇到一堆问题。（此项目是运行在node环境中的，所以要求我们一定要安装好node环境）
- 检查：node -v  npm -v (两个指令)
- 下载的速度慢：可以使用淘宝镜像：npm install cnpm -g --registry=https://registry.npm.taobao.org直接解决
- 如果第一次运行npm install指令报错的话，首先需要手动删除node_moudules，然后到对应项目界面去清除缓存npm cache clean --force（一般第一次运行都不会成功的，可以直接清除缓存到下一步）
- chromedriver@2.27.2报这个错：需要再次删除node_moudules,然后再清除缓存，再运行npm install chromedriver@2.27.2 --ignore-scripts进行安装
- 一般我们使用的sass这个版本都是存在问题的，这一步一般也都需要去做；更新sass版本：npm i node-sass --sass_binary_site=https://npm.taobao.org/mirrors/node-sass/
- 最后再去执行npm run dev即可。
## renren-fast-vue
- renren-fast-vue基于vue、element-ui构建开发，实现[renren-fast](https://gitee.com/renrenio/renren-fast)后台管理前端功能，提供一套更优的前端解决方案
- 前后端分离，通过token进行数据交互，可独立部署
- 主题定制，通过scss变量统一一站式定制
- 动态菜单，通过菜单管理统一管理访问路由
- 数据切换，通过mock配置对接口数据／mock模拟数据进行切换
- 发布时，可动态配置CDN静态资源／切换新旧版本
- 演示地址：[http://demo.open.renren.io/renren-fast](http://demo.open.renren.io/renren-fast) (账号密码：admin/admin)

![输入图片说明](https://images.gitee.com/uploads/images/2019/0305/133529_ff15f192_63154.png "01.png")
![输入图片说明](https://images.gitee.com/uploads/images/2019/0305/133537_7a1b2d85_63154.png "02.png")


## 说明文档
项目开发、部署等说明都在[wiki](https://github.com/renrenio/renren-fast-vue/wiki)中。


## 更新日志
每个版本的详细更改都记录在[release notes](https://github.com/renrenio/renren-fast-vue/releases)中。
