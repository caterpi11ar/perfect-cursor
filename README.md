# perfect-cursor

> 🖱️ **perfect-cursor** 是一个为 [Cursor](https://cursor.com) 设计的最佳实践配置集合，  
> 通过 黄金标准文件（Gold-Standard Files） 与 反馈记忆机制（Feedback Memory Mechanism），让 AI 持续学习并产出更稳定、更优质的代码。

---

## **✨ 1. 黄金标准文件：给 AI 设定质量标杆**

黄金标准文件（Gold-Standard Files）是经过挑选和打磨的 高质量示例文件，它们告诉 AI：
> "这是我们期望的写法，请按这个风格和逻辑来写。"

### **如何创建和维护黄金标准文件？**

1.  **精心选择**：

    - **核心模块**：选择项目中设计最完善、代码最优雅的核心模块作为范例。例如，一个实现了复杂业务逻辑但结构清晰的 `service` 文件。
    - **通用组件**：一个被广泛复用、API 设计精良的 UI 组件或工具函数库。
    - **典型页面**：一个包含了数据获取、状态管理和用户交互的典型页面。

2.  **持续优化**：

    - 在每次重构或需求迭代后，重新审视并更新这些标准文件，确保它们始终代表最新的团队规范。
    - 可以在文件名或文件夹旁加上特殊标记（如 `_gold.ts` 或 `gold-standard/`），以便团队成员和 AI 识别。

3.  **明确注解**：

    - 在这些文件的关键部分添加详细的注释，解释“为什么这么做”。这不仅能帮助新成员理解，也能为 AI 提供更深层次的上下文。

    <!-- end list -->

    ```typescript
    // /src/services/user_service._gold.ts

/**
 * @description 获取用户配置信息.
 * 始终使用 'useSWR' 进行数据获取，以确保自动缓存、请求去重和后台刷新。
 * 这是我们团队处理客户端数据请求的黄金标准。
 * @param userId - 用户的唯一标识符
 */
export function useUserProfile(userId: string) {
  // ... 具体实现
}
```

---

## **✨ 2. 反馈记忆机制：让 AI 从错误中学习**

“反馈记忆机制（Feedback Memory Mechanism）”是将代码审查（Code Review）中反复出现的、共性的反馈意见，转化为 AI 可以理解和遵循的规则库。这能极大地减少重复性纠错的沟通成本。

### **如何构建反馈记忆库？**

1.  **创建 `.cursor/rules` 目录**：
    在项目根目录下创建一个名为 `.cursor` 的文件夹，并在其中建立一个 `rules` 子目录。这里将存放所有 AI 需要学习的规则。

2.  **将反馈转化为 Markdown 文件**：
    - 为每一条常见的反馈创建一个独立的 `.mdc` 文件。文件名应清晰地概括规则内容。
    - 使用简洁、明确的语言描述问题和正确的做法

### **仓库结构建议**

```
.
├── .cursor/
│   └── rules/     # 全局通用规则
│       ├── api-error-handling-standard.mdc
│       └── prefer-type-alias-over-interface.mdc
└── ...
```

---

## **✨ 3. 项目编码规范**

我们的项目遵循以下核心编码规范：

- 使用 **TypeScript** 和 **React** 进行开发
- 严格控制依赖引入，确保打包体积最小化
- 确保代码兼容现代浏览器
- 支持服务端渲染
- 保持 API 向下兼容，避免破坏性变更
- 合理使用 React.memo、useMemo 和 useCallback 优化性能

详细规范请参考 `.cursor/rules` 目录下的具体规则文件。

---