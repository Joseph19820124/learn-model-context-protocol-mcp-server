# 学习模型上下文协议(MCP)服务器

欢迎来到模型上下文协议(Model Context Protocol, MCP)学习仓库！这里收集了关于MCP的中文学习资源、翻译文档和实践指南。

## 🎯 仓库目标

- 📚 提供MCP相关的中文学习资源
- 🌐 翻译优质的英文MCP文档和教程
- 💡 分享MCP实践经验和最佳实践
- 🔧 收集MCP服务器和客户端的实现示例

## 📖 内容目录

### 📄 翻译文档

- [Make.com MCP服务器指南](make-mcp-server-guide.md) - Make.com官方博客关于MCP服务器的完整指南翻译

### 🔗 推荐资源

**官方资源：**
- [Anthropic MCP官方介绍](https://www.anthropic.com/news/model-context-protocol)
- [MCP GitHub仓库](https://github.com/modelcontextprotocol)
- [MCP规范文档](https://spec.modelcontextprotocol.io/)

**实用工具：**
- [Claude Desktop](https://claude.ai/desktop) - 支持MCP的AI客户端
- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) - MCP服务器测试工具

## 🚀 快速开始

### 什么是MCP？

模型上下文协议(Model Context Protocol)是一个开放标准，用于连接AI模型与外部工具、数据源和系统。它就像AI集成的"USB标准"，解决了AI应用与外部服务集成的复杂性问题。

### MCP的核心优势

- **🔄 标准化**：统一的协议替代碎片化的集成方式
- **🛠️ 工具箱**：为AI提供丰富的外部工具和数据访问能力
- **🔒 安全性**：内置访问控制和标准化安全实践
- **📈 可扩展性**：轻松添加新的功能和服务

### 主要组件

1. **MCP客户端** - 集成在AI应用中，如Claude Desktop
2. **MCP服务器** - 提供特定功能的独立服务，如GitHub集成、数据库访问等
3. **传输层** - 客户端和服务器之间的通信机制

## 🏗️ 架构概览

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   AI应用/客户端   │◄──►│   MCP协议层      │◄──►│   MCP服务器      │
│                 │    │                 │    │                 │
│ • Claude        │    │ • JSON-RPC 2.0  │    │ • GitHub        │
│ • Cursor IDE    │    │ • STDIO/HTTP    │    │ • Slack         │
│ • 自定义应用     │    │ • 工具发现       │    │ • 数据库        │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

## 📚 学习路径

### 初学者
1. 阅读 [Make.com MCP服务器指南](make-mcp-server-guide.md)
2. 了解MCP的基本概念和架构
3. 安装Claude Desktop并配置第一个MCP服务器

### 进阶用户
1. 学习如何创建自定义MCP服务器
2. 探索不同的传输方式(STDIO vs HTTP)
3. 实现复杂的工具和资源

### 开发者
1. 研究MCP规范和SDK
2. 构建生产级MCP服务器
3. 贡献到MCP开源生态系统

## 🤝 贡献指南

我们欢迎各种形式的贡献：

- 📝 翻译优质的英文MCP文档
- 💡 分享MCP使用经验和案例
- 🐛 报告文档错误或提出改进建议
- 🔧 提供代码示例和最佳实践

### 如何贡献

1. Fork这个仓库
2. 创建你的特性分支 (`git checkout -b feature/amazing-feature`)
3. 提交你的更改 (`git commit -m 'Add some amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 打开一个Pull Request

## 📞 联系方式

- GitHub Issues: [提出问题或建议](https://github.com/Joseph19820124/learn-model-context-protocol-mcp-server/issues)
- Discussions: [参与讨论](https://github.com/Joseph19820124/learn-model-context-protocol-mcp-server/discussions)

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🌟 感谢

感谢以下项目和组织推动MCP的发展：
- [Anthropic](https://www.anthropic.com/) - MCP的创建者
- [Make.com](https://www.make.com/) - 提供优质的MCP实践指南
- MCP开源社区的所有贡献者

---

⭐ 如果这个仓库对你有帮助，请考虑给它一个星标！