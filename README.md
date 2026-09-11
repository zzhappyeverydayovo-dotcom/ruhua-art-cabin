# 入画 · 下一百廿年

全息舱交互演示与技术对接资料。

## 下载完整项目

请打开 [最新发行版](https://github.com/zzhappyeverydayovo-dotcom/ruhua-art-cabin/releases/latest)，下载 `ruhua-complete.zip`，包含完整源码、界面图片、首页视频和32张海报。

仓库中的 `ruhua-source.zip` 仅包含源码；运行请下载上面的完整发行包。

## 运行

安装 Node.js 22.13 或更新版本。解压完整包，进入 ruhua-system 目录：

```sh
npm ci
npm run dev
```

`npm run build` 生成 dist/client，可部署到静态 HTTP 服务器。

## 交互流程

首页视频 → 男生/女生形象 → 四方向或八身份 → 等待 → 海报预览与换图 → 保存方式。

此版本是海报模板演示，尚未连接摄像头、人脸识别、真实AI生成及正式二维码服务。Unity制作参考完整包内README及public/handoff.html。
