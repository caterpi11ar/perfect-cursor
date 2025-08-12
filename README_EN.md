# Perfect Cursor

> 🖱️ **Perfect Cursor** is a **best practice configuration collection** built for [Cursor](https://cursor.com).  
> Through **Gold-Standard Files** + **Feedback Memory Mechanism**,  
> it enables AI to continuously learn and produce more stable, higher-quality code.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Cursor Version](https://img.shields.io/badge/Cursor-Required-blue.svg)](https://cursor.com)
[![Documentation](https://img.shields.io/badge/Documentation-Complete-green.svg)](./CONFIGURATION_EN.md)
[![中文](https://img.shields.io/badge/中文-README_CN.md-red.svg)](./README_CN.md)

---

## ✨ Features

- 🎯 **Gold-Standard Files** - Set quality benchmarks for AI
- 🧠 **Feedback Memory Mechanism** - Let AI evolve from mistakes  
- 📚 **Project Coding Standards** - Unified development standards
- 🚀 **Quick Start** - Simple and easy configuration process
- 🔧 **TypeScript Support** - Complete type definition specifications
- 🧪 **Testing Standards** - Unified testing standards and processes
- 📝 **Git Workflow** - Standardized version control processes

---

## 🚀 Quick Start

### Prerequisites

- [Cursor](https://cursor.com) editor
- Basic project configuration experience

### Installation & Configuration

1. **Clone the project**
   ```bash
   git clone https://github.com/caterpi11ar/perfect-cursor.git
   cd perfect-cursor
   ```

2. **Configure rules**
   - Add or update rule files in `.cursor/rules/`
   - Regularly review and update gold-standard files
   - Before adding new modules, refer to gold-standard examples

3. **During Code Review**
   - Precipitate frequent feedback into the rule library

---

## 📁 Project Structure

```
perfect-cursor/
├── .cursor/                    # Cursor editor configuration directory
│   └── rules/                  # Rule files directory
│       ├── workflow.mdc        # Workflow specifications
│       ├── project.mdc         # Project development standards
│       ├── typescript.mdc      # TypeScript specifications
│       ├── common.mdc          # Common development standards
│       ├── demo.mdc            # Demo code standards
│       ├── git.mdc             # Git workflow standards
│       └── testing.mdc         # Testing standards
├── README_EN.md                # English project documentation
├── CONFIGURATION_CN.md         # Chinese configuration documentation
├── CONFIGURATION_EN.md         # English configuration documentation
└── ...                         # Other project files
```

---

## 🔧 Configuration

### Gold-Standard Files

**Gold-Standard Files** are carefully selected **high-quality code examples** that tell AI:
> "This is the style and logic we expect, please refer to and maintain consistency."

#### Creation and Maintenance Steps

1. **Carefully Select Examples**
   - **Core Modules**: Well-structured, well-designed core business modules
   - **Common Components**: Elegantly designed APIs, UI components or utility function libraries reused in multiple places
   - **Typical Pages**: Complete pages containing data fetching, state management and interaction logic

2. **Continuous Optimization**
   - Update these files after each refactoring or requirement iteration
   - Files can be marked with special tags for easy identification by teams and AI

3. **Add Clear Annotations**
   - Add explanations for **why to do this** at key implementations
   - Comments help both new members and provide context for AI

### Feedback Memory Mechanism

**Feedback Memory Mechanism** precipitates **common problems** that repeatedly appear in Code Review into **rule files** that AI can directly understand, reducing repetitive corrections.

#### Building Feedback Memory Library

1. **Create Rules Directory**
   ```bash
   mkdir -p .cursor/rules
   ```

2. **Convert Feedback to Rules**
   - Write each common feedback as a separate `.mdc` file
   - Filenames should be concise and clear
   - Rule descriptions should be concise, clear and directly executable

---

## 📚 Documentation

- 📖 [Configuration Guide](./CONFIGURATION_EN.md) - Detailed configuration guide (English)
- 📖 [配置说明](./CONFIGURATION_CN.md) - 详细的配置指南（中文）
- 📋 [Coding Standards](./.cursor/rules/) - Project coding rules
  - [Workflow Standards](./.cursor/rules/workflow.mdc)
  - [Project Development Standards](./.cursor/rules/project.mdc)
  - [TypeScript Specifications](./.cursor/rules/typescript.mdc)
  - [Common Development Standards](./.cursor/rules/common.mdc)
  - [Git Workflow Standards](./.cursor/rules/git.mdc)
  - [Testing Standards](./.cursor/rules/testing.mdc)

---

## 🎯 Use Cases

- **Team Development** - Unify code style and development standards
- **AI-Assisted Development** - Guide AI to generate quality code through rule files
- **Code Review** - Reduce repetitive issues and improve review efficiency
- **Newcomer Training** - Quickly understand project development standards and best practices
- **Project Maintenance** - Maintain code quality and consistency

---

## ✅ Quick Start Checklist

* [ ] Add or update rule files in `.cursor/rules/`
* [ ] Regularly review and update gold-standard files
* [ ] Before adding new modules, refer to gold-standard examples
* [ ] During Code Review, precipitate frequent feedback into the rule library
* [ ] Follow TypeScript specifications and Git workflow
* [ ] Write test cases according to testing standards

---

## 🤝 Contributing

We welcome all forms of contributions! Please check our [Contributing Guide](.github/CONTRIBUTING.md) for details.

### Types of Contributions

- 🐛 Report Bugs
- 💡 Suggest New Features
- 📝 Improve Documentation
- 🔧 Submit Code Fixes
- 🧪 Add Test Cases
- 📚 Improve Rule Files

### Contribution Process

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

Thanks to all developers and users who have contributed to this project!

Special thanks to:
- [Cursor](https://cursor.com) team for providing an excellent editor
- All contributors and users for their support and feedback

---

## 🌐 Multi-language Support

- 🇨🇳 [Chinese Version](./README.md) - 中文版本
- 🇺🇸 [English Version](./README_EN.md) - Current page

---

<div align="center">
  <p>If this project helps you, please give it a ⭐️</p>
  <p>Made with ❤️ for the Cursor community</p>
</div>
