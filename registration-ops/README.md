# Medxpert Registration Ops（注册准入作战团）

医疗器械注册运营团队：注册领航员领衔，统筹 AI 器械合规、ISO 13485 质量体系、国际市场准入与注册策略，输出完整注册路线图。覆盖 NMPA / FDA / CE / 日本 PMDA / 东盟·拉美·中东等多国路径，以及 SaMD、EU AI Act、PCCP、ISO/IEC 42001 等 AI 合规议题。

## 类型

Team 型（多角色协作团队）：注册领航员（主理人）+ 合规官 + 文控官 + 出海官。

## 功能

- 四线并行 SOP：AI 合规探路 → 国际准入探路 → 主路径裁定 → 体系/文档差距 → 路线图汇编
- 产出：注册路线图、主路径裁定书、合规差距报告、分国别准入路线图（七栏制）、CE 技术文件与 GSPR 矩阵、ISO 13485 四级文件体系、CAPA 闭环、迎审问题库
- 知识底座：配套安装 MedXpert 医械注册知识库 v0.7（L0–L4，含判定引擎与法规时间轴）

## 使用示例

- 「我们一款带 AI 辅助诊断的影像软件，想先进欧盟再进东南亚，体系文件只有一版旧质量手册，帮我出注册路线图」
- 「这款 AI 器械走 510(k) 还是 De Novo？」
- 「做一份沙特 SFDA 注册准入路线图」
- 「ISO 13485 四级文件从零搭一套」
- 「下个月 MDR 公告机构来审，帮我出问题库」

## 头像

头像已生成在 `avatars/` 目录下。

## 安装

将专家包目录放到专家目录下：

```
C:\Users\<用户名>\.workbuddy\plugins\marketplaces\my-experts\plugins\medxpert-registration-ops\
```

安装后由 WorkBuddy 开放平台自动注册并可见；如本地手动导入，将该目录置于专家插件目录下即可，无需额外脚本。

## 知识库配套（可选但推荐）

本团队为方法论层，事实以 MedXpert 医械注册知识库 v0.7 为准。如需引用具体法规原文、国别路径与判定引擎，请另行安装该知识库配套包。

## 打包分享

```bash
zip -r medxpert-registration-ops.public.zip medxpert-registration-ops/
```

## 版权与免责声明

© 2026 MedXpert（https://medxpert.cn）。本专家包以 MIT 许可发布。
本包按「现状」（AS IS）提供，不含任何明示或暗示担保；输出仅供方法论参考，不构成法规、法律或医疗建议。具体注册决策以正式申报及监管机构最终意见为准。

<!-- BOUNDARY-20260908 -->

## 边界与分工（注册线）

**本包定位**：**注册执行团**。接单后的项目运营：资料清单、进度与 deadline 管理、跨方协调。

**同组分工**：
- `medical-device-reg-expert`：**咨询顾问（第一入口）**。面向客户的分类判定、注册路径建议、标准解读、方案沟通。
- `medxpert-registration-ops`：**注册执行团**。接单后的项目运营：资料清单、进度与 deadline 管理、跨方协调。 ← 本包
- `medxpert-reg-translator`：**注册文档翻译**。中英注册资料互译与医械法规术语一致性；不做法规判断。

**路由规则**：客户问「怎么注册/多少钱/什么分类」→ reg-expert；确定立项做注册 → registration-ops；只需翻译资料 → reg-translator。
