# CHANGELOG

All notable changes to Synapse Skills will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-04-08

### Added

#### synapse-wiki (智能知识库管理系统)
- **核心功能**:
  - `wiki_init` — 初始化新的 Wiki 知识库
  - `wiki_ingest` — 摄取源文件创建 Wiki 页面
  - `wiki_query` — 查询知识并综合答案
  - `wiki_lint` — 健康检查（死链接、孤立页面等）
- **Scripts**:
  - `scaffold.py` — 引导新的 Wiki 目录树
  - `ingest.py` — 摄取新资料，编译为 Wiki 页面
  - `query.py` — 查询 Wiki，综合答案
  - `lint_wiki.py` — 健康检查（死链接/孤立页/矛盾）
- **Commands**: `init.sh`, `ingest.sh`, `query.sh`, `lint.sh`
- **Tests**: 基线测试 4/4 通过

### Changed

- SKILL.md 描述优化，突出"越用越聪明"的核心价值
- 移除技术术语（LLM Wiki、RAG 对比），改用用户友好语言
- 安装脚本支持 --dry-run 和 --uninstall

### Fixed

- 目录结构统一，所有元数据文件位于根目录
- 配置文件支持 config.template.json → config.json 自动创建

### Security

- 无

---

## [0.1.0] - 2026-04-08 (Initial Draft)

### Added

- 初始版本创建
- 基线测试框架
