# 未来小小工程师增量包 · 2026-09-14

本包仅新增工程师模块，不包含或替换已由全息舱技术人员对接的未来艺术家模块。请在技术方当前工程中合并。

## 接入
1. 将 additions 下的 components、lib、public 合并到当前项目同名目录，均为工程师新增文件。
2. integration/engineer-entry.patch 只包含 app/page.tsx 的双入口接入改动。请按差异手动合并到已对接版本，不要用旧版整页覆盖技术方当前代码。新增 import、branch 状态、首页开启入口和工程师渲染分支；保持艺术家服务与现有生成、下载、设备逻辑。
3. 在现有配置中新增 engineerEndpoint 字段（未对接时为空字符串），不要覆盖 generationEndpoint、posters 或其他配置。
4. 本模块复用现有 lib/flow 的 parseResult、safeUrl 和 Result，以及 React / lucide-react。无需新增二维码依赖。

## 已完成
男女儿童选择；进入拍照页自动开启摄像头；仅现场拍摄和重拍；四种身份每轮不重复；八张儿童海报；保存后进入独立扫码页，二维码位置显示“二维码待接入”。服务端返回 downloadQr 后可显示正式二维码。

相机首次需要授权，运行环境需 HTTPS 或 localhost。当前未接真人AI生成，照片不上传；接入 engineerEndpoint 后才发送照片。外屏接收仍由技术方接入。

协议见 ENGINEER-HANDOFF.md。交付前已通过 TypeScript 检查和生产构建。
