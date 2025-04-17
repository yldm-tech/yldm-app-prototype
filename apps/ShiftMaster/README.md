# ShiftMaster 排班管理系统原型

这是一个用于管理员工排班的系统原型。所有页面都是静态HTML文件。

## 功能概述

- 排班表查看和管理
- 员工班次分配
- 休假申请处理
- 工时统计报表
- 班次模板管理

## 页面说明

- **首页** (index.html): 主控制面板和排班表

## 运行项目

本项目是静态HTML原型，使用serve静态文件服务器运行：

```bash
# 安装依赖
pnpm install

# 启动静态服务器
pnpm start
```

启动后，应用将在 http://localhost:3000 可访问。

也可以通过根目录的命令启动：

```bash
# 在根目录执行
pnpm start:shift
``` 