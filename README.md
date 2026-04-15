# 📚 图书管理系统 (Library Management System)

> 🎮 **个人练手项目** | 🧸 **小玩具** | 📝 **课程作业**

基于 Python tkinter 开发的桌面图书管理系统，实现图书信息的增删改查功能。

## ✨ 功能特性

- 🔐 **用户登录** - 简单的身份验证机制
- 📖 **图书录入** - 添加新图书信息（图书号、书名、作者、出版社）
- 🔍 **图书查询** - 表格形式展示所有图书，支持刷新
- ✏️ **图书修改** - 根据书名查询并修改图书信息
- 🗑️ **图书删除** - 根据书名删除图书记录

## 🛠️ 技术栈

| 类别 | 技术 |
|------|------|
| GUI框架 | tkinter |
| 数据存储 | JSON 文件 |
| 开发语言 | Python 3 |

## 📁 项目结构

```
图书管理系统/
├── LoginPage.py     # 登录界面
├── MainPage.py      # 主界面与菜单导航
├── views.py         # 各功能模块界面
│   ├── SearchFrame  # 查询界面
│   ├── InsertFrame  # 录入界面
│   ├── ChangeFrame  # 修改界面
│   ├── DeleteFrame  # 删除界面
│   └── AboutFrame   # 关于界面
├── db.py            # 数据库操作类
├── books.json       # 图书数据存储
└── users.json       # 用户数据存储
```

## 🚀 快速开始

### 环境要求

- Python 3.x
- 无需安装额外依赖（tkinter 为 Python 标准库）

### 运行方式

```bash
# 克隆仓库
git clone https://github.com/29061/tkinter-library-management-system.git
cd tkinter-library-management-system/图书管理系统

# 运行程序
python LoginPage.py
```

### 默认账户

| 用户名 | 密码 |
|--------|------|
| admin | 123456 |

> 密码存储在 `users.json` 文件中，可根据需要修改。

## 📸 界面预览

### 登录界面
- 输入用户名和密码进行身份验证

### 主界面
- 菜单栏包含：录入、查询、删除、修改、关于
- 各功能模块通过菜单切换

## 💾 数据说明

数据以 JSON 格式存储在本地文件中：

**books.json** - 图书数据
```json
[
    {
        "id": "001",
        "bookname": "书名",
        "author": "作者",
        "press": "出版社"
    }
]
```

**users.json** - 用户数据
```json
{
    "username": "admin",
    "password": "123456"
}
```

## 📝 开发说明

本项目主要用于：
- 练习 Python tkinter 基本语法
- 学习 GUI 程序开发流程
- 了解简单的数据持久化方案
- 可用作学校课程作业参考

## 📄 许可证

本项目采用 MIT 许可证。

---

<p align="center">
  <i>一个简单的图书管理小工具，适合 Python GUI 入门学习 🎉</i>
</p>
