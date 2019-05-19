# HexoBlogClient


[![Gitter](https://img.shields.io/gitter/room/Xonlystar/hexo-blog-client.svg)](https://gitter.im/hexo-blog-client/Lobby?utm_source=badge) 
[![GitHub issues](https://img.shields.io/github/issues/Xonlystar/hexo-blog-client.svg)](https://github.com/Xonlystar/hexo-blog-client/issues) 
[![GitHub license](https://img.shields.io/github/license/Xonlystar/hexo-blog-client.svg)](https://github.com/Xonlystar/hexo-blog-client/blob/master/LICENSE) 
[![Download](https://img.shields.io/badge/downloads-master-green.svg)](https://codeload.github.com/Xonlystar/hexo-blog-client/zip/master) [![Hexo Version](https://img.shields.io/badge/hexo-%3E%3D%203.0-blue.svg)](http://hexo.io) 
[![GitHub forks](https://img.shields.io/github/forks/Xonlystar/hexo-blog-client.svg)](https://github.com/Xonlystar/hexo-blog-client/network) 
[![GitHub stars](https://img.shields.io/github/stars/Xonlystar/hexo-blog-client.svg)](https://github.com/Xonlystar/hexo-blog-client/stargazers)

 [English Document](./README_EN.md) | [个人博客](https://blog.onlystar.site) | QQ 交流群: `212388109`
> HexoBlogClient是一个采用`Electron + Vue`开发的Hexo博客管理客户端，基于[HexoClient](https://github.com/gaoyoubo/hexo-client.git)二次开发

## 特性
  - 简单漂亮，文章易读易修改
  - 支持文章置顶显示
  - 博客文章的增删改查
  - 文章支持七牛图片上传
  - 支持hexo generate
  - 支持hexo deploy

## 后续开发计划
- [x] 搜索文章, 分类以及标签搜索
- [x] 软件设置
- [x] 一键编译、发布博客
- [x] 检查软件更新
- [ ] 将文章保存为草稿
- [ ] 优化关键词交互
- [ ] 本地预览博客
- [ ] 自动保存文章
- [ ] 软件消息提示
- [ ] 操作日志记录

## 开发
使用`git clone`下载到本地开发
```bash
git clone https://github.com/Xonlystar/hexo-blog-client.git
```
安装依赖并运行
```bash
# 使用npm 安装依赖
npm install

# 开发模式
npm start

# 打包
npm run build
```

更换icon图标
```bash
# 安装
npm install --save-dev electron-icon-builder

# scripts中添加
"generate-icons": "electron-icon-builder --input=./public/icon.png --output=build --flatten"
```
## [配置](https://blog.onlystar.site/2018/10/21/hexoblogclient-shi-yong-zhi-nan/)

## 效果截图

![列表页](https://user-images.githubusercontent.com/19361551/57982641-93749280-7a7a-11e9-9dd8-485943d71f78.png)
![列表页-伸展](https://user-images.githubusercontent.com/19361551/57982663-054cdc00-7a7b-11e9-8251-48c94fddc6be.png)
![分类页](https://user-images.githubusercontent.com/19361551/57982655-f5cd9300-7a7a-11e9-9566-5da49f1b3d77.png)
![标签页](https://user-images.githubusercontent.com/19361551/57982661-01b95500-7a7b-11e9-8b63-f4726d9a30d1.png)
![筛选页](https://user-images.githubusercontent.com/19361551/57982697-712f4480-7a7b-11e9-88c5-268f22bfccd2.png)
![关于页](https://user-images.githubusercontent.com/19361551/57982878-9fae1f00-7a7d-11e9-9061-0d0a05b11844.png)
![配置页](https://user-images.githubusercontent.com/19361551/57982906-11866880-7a7e-11e9-9537-f0a42d4a0ab4.png)
![新增文章页](https://user-images.githubusercontent.com/19361551/57982917-1f3bee00-7a7e-11e9-8107-a8022116f0a0.png)
![文章配置](https://user-images.githubusercontent.com/19361551/57982991-362f1000-7a7f-11e9-9800-eb49309584a4.png)
![修改文章页](https://user-images.githubusercontent.com/19361551/57982954-c3259980-7a7e-11e9-9689-729b3f519a44.png)

## 版本更新记录
### v1.2.7 (2019-05-20)
- 新增Front-Matters编辑功能
- 新增同步git仓库文章功能
- 优化文章搜索功能，大小写字母皆可模糊搜索
- 新增检查更新功能
- 新增博客链接地址配置，可打开博客
- 修复左侧文章列表宽度显示偶尔变动的问题
- 修复linux下图标缺失的问题
- 修复linux下系统托盘显示异常的问题
- Mac新增Touchbar功能(试验性功能)
- 支持两种语言：中文和英文

### v1.2.6 (2019-05-16)
- 新增markdown编辑器快捷键(ctrl + s)保存功能
- 升级markdown编辑器版本
- 修复https://sm.ms图床设置不生效的问题
- 支持常用快捷键操作
- 修复部分情况预览文章空白的问题
- 修复偶尔发布博客失败的问题

### v1.2.5 (2019-04-24)
- 更新界面，参考有道云笔记
- 支持更换头像，可以自定义上传daogit
- 支持最小化到系统任务栏
- 支持分类和标签搜索
- 支持分类和标签的列表展示以及各自对应的文章条数