# skill

[English](./README.md) | 中文

个人 Claude Code skill 合集 —— 经过实际项目验证，可直接用于任何项目。

---

## 安装方式

使用 `skills` CLI 安装任意 skill：

```bash
npx skills@latest add paullu03/skill/skills/<skill-name>
```

---

## Skills 列表

### [choose-awesome-design](./skills/choose-awesome-design/)

UI 原型设计风格顾问。在向你提问之前，它会先自动扫描项目中的设计文档、PRD、README、架构文档等，理解你的产品背景。随后通过多轮对话，从四个维度逐步了解你的需求：目标用户、产品类型、视觉氛围和参考品牌。最终从 [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) 的 58 个品牌设计规范中推荐 2–3 个最匹配的方案，并对比各自适合的场景。确认选择后，自动从 GitHub 拉取对应的 `DESIGN.md`，作为本次会话中所有 UI 工作的设计规范。

```bash
npx skills@latest add paullu03/skill/skills/choose-awesome-design
```

---

## 关于本仓库

这是个人仓库，skill 会在实际项目中验证有用后持续添加。
