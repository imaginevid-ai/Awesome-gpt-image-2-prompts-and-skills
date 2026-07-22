# awesome-gpt-image-2-prompts-and-skills
GPT Image 2 Library 品牌的 GPT Image 2 prompts and skills 公开资料仓库。

<directory>
data/ - GPT Image 2 分类、83 条社区案例与官方案例的结构化真源。
docs/ - 规划、贡献指南、本地开发说明与后续数据采集策略。
public/images/ - 仓库 README 与社交预览图，必须使用 GPT Image 2 Library 自有生成图。
scripts/ - README 生成、数据导入、Issue 同步与后续 twitterapi.io 采集脚本。
.github/ - Issue 模板、labels 与 GitHub Actions。
</directory>

<config>
AGENTS.md - 仓库级工程约束。
</config>

## 产品定位
- 目标仓库为 `imaginevid-ai/Awesome-gpt-image-2-prompts-and-skills`。
- 品牌使用 `GPT Image 2 Library`，不要出现 reference repository 口吻、reference repository 链接或 reference repository 图片资产。
- 参考仓库 `the reference repository` 只作为结构样板。
- 不接外部 CMS 或独立图库；本仓库只用本地采集/归一化数据生成 README 并推送远端。

## 开发规范
- README 结构、Issue 提交流程、labels 与定时生成机制可对齐参考仓库。
- 所有展示文案必须重写为 GPT Image 2 / GPT Image 2 Library 语境。
- README 中涉及 GPT Image 2 能力的说明必须有 OpenAI 官方文档依据；项目入口链接保持指向本仓库。
- 所有封面图、OG 图、示例图必须重新生成或使用授权资产，不直接复用参考仓库图片。
- 数据源字段需要保留原作者、原帖链接、发布时间、语言、分类、媒体 URL 与审核状态。
- 数据结构优先镜像参考仓库的 `Prompt`、`PromptCategory`、`FilterCategory`，不要为假想平台额外扩 schema。
- 后续使用 twitterapi.io 时只读取本地 skill 配置或环境变量，不提交 API key、cookies、proxy、原始大批量抓取缓存。
- twitterapi.io 搜索结果必须先通过 `quality:twitter` 评分、人工来源核验和媒体感知去重；关键词命中不能直接进入公开数据。
- 引用外部提示词仓库时必须核对许可证，并在 README、数据来源字段和原作者链接中保留署名。

## 计划边界
- 当前阶段已经生成仓库文件、图片资产、采集脚本、GitHub Actions 与本地数据。
- 提交前必须重新运行 `pnpm run generate`、`pnpm test`、`pnpm run typecheck`，并确认没有提交 twitterapi.io 原始抓取缓存。
