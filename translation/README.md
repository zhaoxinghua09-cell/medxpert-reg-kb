# Medical Device Reg Translator（医械法规翻译专家）





> **🌐 官网：https://medxpert.cn/knowledge/**（医械注册知识库·免费公开层）





医械法规文件专业翻译专家（Agent 型），中英互译，专注 FDA 510(k)/PMA、CE MDR 技术文件、IFU、标签、临床报告、质量体系文档的翻译与润色。与「医械注册法规专家」（咨询定位）互补——本专家负责**翻译交付**。





## 类型





Agent 型（单个 AI 专家）





## 功能





- **法规文档中英互译**：IFU/使用说明书、510(k)/PMA、CE MDR 技术文件、标签、临床评价报告、质量文档、出口销售证明


- **术语一致性管理**：先建术语表再翻译，标准号/法规名/机构名不翻译，警示语义不弱化


- **市场语境区分**：NMPA/FDA/MDR/PMDA 术语体系差异精确处理（如 clearance vs approval）


- **格式还原与交付**：表格/编号/章节结构保留，双语对照或目标语言交付





## 知识底座





- `medical-device-reg-translation` 技能（翻译工作流 + 医械中英术语对照表 + 文档类型翻译要点）


- 与 `medical-device-reg-hub`（26 枢纽图书馆）同源，法规术语与官方链接以枢纽为准





## 使用示例





- 帮我翻译这份 FDA 510(k) 文件（中译英）


- 帮我校对这份 IFU 的法规术语一致性


- 为 CE MDR 技术文件翻译建一份术语表





## 头像





头像已自动生成在 `avatars/` 目录下。如需替换为自定义头像，要求：


- 格式：PNG（推荐）或 JPG


- 尺寸：512×512 px


- 大小：单张不超过 500KB





## 安装





将专家包目录放到专家目录下：





```


~\.workbuddy\plugins\marketplaces\my-experts\plugins/medical-device-reg-translator/


```





然后运行注册命令使其可见：





```bash


python3 scripts/register_expert.py <expert-dir>


```





## 打包分享





```bash


zip -r medical-device-reg-translator.zip medical-device-reg-translator/


```





## 版权与许可





- © 2026 **注册老炮@MedXpert**。以 **MIT 协议**开源发布。


- **免责声明**：本专家按「现状（AS IS）」提供，不提供任何明示或默示的担保；因使用、误用本专家或其输出导致的任何直接或间接损失，作者不承担责任。


- 内容仅供合规工作参考，不构成法规意见、法律意见或注册代理服务。



<!-- BOUNDARY-20260908 -->

## 边界与分工（注册线）

**本包定位**：**注册文档翻译**。中英注册资料互译与医械法规术语一致性；不做法规判断。

**同组分工**：
- `medical-device-reg-expert`：**咨询顾问（第一入口）**。面向客户的分类判定、注册路径建议、标准解读、方案沟通。
- `medxpert-registration-ops`：**注册执行团**。接单后的项目运营：资料清单、进度与 deadline 管理、跨方协调。
- `medxpert-reg-translator`：**注册文档翻译**。中英注册资料互译与医械法规术语一致性；不做法规判断。 ← 本包

**路由规则**：客户问「怎么注册/多少钱/什么分类」→ reg-expert；确定立项做注册 → registration-ops；只需翻译资料 → reg-translator。
