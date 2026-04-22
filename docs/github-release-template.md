# GitHub Release 文案模板

## 使用方式

每次发版时，复制下面的模板到 GitHub Release 描述框，再按当前版本内容替换占位文本。

## 通用模板

```md
## Overview

本次版本聚焦于 [一句话说明本次版本解决的核心问题]。

## Highlights

- [亮点 1：新增了什么能力]
- [亮点 2：优化了什么流程]
- [亮点 3：补齐了什么长期治理或稳定性问题]

## Changes

### Added

- [新增项 1]
- [新增项 2]

### Changed

- [调整项 1]
- [调整项 2]

### Fixed

- [修复项 1]
- [修复项 2]

## Impact

- 是否影响公开入口： [是 / 否]
- 是否影响协作流程： [是 / 否]
- 是否需要迁移操作： [是 / 否]

## Upgrade Notes

- [如果无需迁移，写“无特殊升级步骤”]
- [如果有目录、规则或配置变化，在这里说明]

## Verification

- [验证动作 1]
- [验证动作 2]

## Links

- Changelog: [CHANGELOG.md](<仓库中的 changelog 链接>)
- Docs: [docs/README.md](<仓库中的 docs 链接>)
- Tag: [vX.Y.Z](<当前 tag 链接>)
```

## 精简模板

适合 `PATCH` 版本，内容不多时可以直接用：

```md
## Overview

本次版本主要完成了 [一句话总结]。

## Changes

- [变更 1]
- [变更 2]
- [变更 3]

## Verification

- [验证方式]

## Links

- Changelog: [CHANGELOG.md](<仓库中的 changelog 链接>)
- Tag: [vX.Y.Z](<当前 tag 链接>)
```

## 编写建议

- 第一段先写“为什么发这个版本”，不要一开始就堆文件名
- `Highlights` 只保留 3 条左右，方便仓库访客快速扫读
- `Changes` 与 `CHANGELOG.md` 保持同一口径，但可以更偏对外表达
- 如果是长期治理类版本，明确说明它解决了什么维护成本问题
