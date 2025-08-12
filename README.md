# perfect-cursor

> 🖱️ **perfect-cursor** 是一个为 [Cursor](https://cursor.com) 打造的**最佳实践配置集合**。  
> 通过 **黄金标准文件（Gold-Standard Files）** + **反馈记忆机制（Feedback Memory Mechanism）**，  
> 让 AI 持续学习并产出更稳定、更高质量的代码。

---

## ✨ 1. 黄金标准文件 — 给 AI 设定质量标杆

**黄金标准文件**是精挑细选的**高质量代码示例**，它告诉 AI：
> “这是我们期望的风格与逻辑，请参考并保持一致。”

### 📌 创建与维护步骤

1. **精心选择示例**
   - **核心模块**：结构清晰、设计完善的核心业务模块（如复杂业务逻辑的 `service` 文件）。
   - **通用组件**：API 设计优雅、被多处复用的 UI 组件或工具函数库。
   - **典型页面**：包含数据获取、状态管理与交互逻辑的完整页面。

2. **持续优化**
   - 每次重构或需求迭代后，更新这些文件，确保始终代表**最新团队规范**。
   - 文件可加特殊标记（如 `_gold.ts` 或放入 `gold-standard/` 文件夹），方便团队与 AI 快速识别。

3. **添加明确注解**
   - 在关键实现处，添加说明**为什么这么做**。
   - 注释既能帮助新成员，也能为 AI 提供上下文参考。

```ts
    // /src/services/user_service._gold.ts

    /**
     * @description 获取用户配置信息
     * 始终使用 'useSWR' 进行数据获取，以确保自动缓存、请求去重和后台刷新。
     * 这是我们团队处理客户端数据请求的黄金标准。
     * @param userId - 用户唯一标识符
     */
    export function useUserProfile(userId: string) {
    // ... 具体实现
    }
```

---

## ✨ 2. 反馈记忆机制 — 让 AI 从错误中进化

**反馈记忆机制（Feedback Memory Mechanism）**
将 Code Review 中反复出现的**共性问题**，沉淀为 AI 可直接理解的**规则文件**，减少重复性纠错。

### 📌 构建反馈记忆库

1. **创建规则目录**

```bash
   mkdir -p .cursor/rules
```

   所有规则文件统一存放在 `.cursor/rules/` 下。

1. **将反馈转化为规则**

   * 每条常见反馈写成独立的 `.mdc` 文件。
   * 文件名简明扼要，如：`api-error-handling-standard.mdc
        prefer-type-alias-over-interface.mdc`

   * 规则描述应简洁、明确，可直接执行。

### 💡 推荐目录结构

```csharp
.
├── .cursor/
│   └── rules/     # 全局通用规则
│       ├── api-error-handling-standard.mdc
│       └── prefer-type-alias-over-interface.mdc
└── ...

```

---

## ✨ 3. 项目编码规范


📂 **详细规范**请参考 `.cursor/rules` 中的具体规则文件。

---

## ✅ 快速上手清单

* [ ] 在 `.cursor/rules/` 中添加或更新规则文件
* [ ] 定期审查并更新黄金标准文件
* [ ] 新增模块前，先参考黄金标准示例
* [ ] Code Review 时，将高频反馈沉淀到规则库

---
