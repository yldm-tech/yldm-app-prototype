# YLDM 应用原型集合

这是一个包含多个独立应用原型的项目，使用 pnpm 工作空间进行管理。所有应用都是静态HTML文件，使用serve静态服务器启动。

## 项目结构

```
yldm-app-prototype/
├── apps/                  # 应用集合目录
│   ├── RentHouse/         # 租房小程序高保真原型
│   ├── ShiftMaster/       # 排班管理应用
│   ├── JaDict/            # 日语词典应用
│   └── AnyGallery/        # 任意图库应用
├── node_modules/          # 依赖包
├── package.json           # 根项目配置
└── pnpm-workspace.yaml    # 工作空间配置
```

## 应用说明

### RentHouse (租房小程序)

一个高保真的租房应用原型，展示了用户浏览房源、预订、管理个人资料等功能。

**主要功能**:
- 房源和空间列表浏览
- 房间详情查看
- 预订管理
- 个人中心（收藏、订单、优惠券等）
- 消息中心
- 维修请求

### ShiftMaster (排班管理)

排班管理应用原型，用于人员排班的管理。

### JaDict (日语词典)

日语学习词典应用，包含查询、学习和测验功能。

**主要功能**:
- 单词查询与详情
- AI 辅助搜索
- 收藏夹
- 学习进度跟踪
- 每日学习
- 词汇测验

### AnyGallery (任意图库)

iOS风格的图库应用原型，支持浏览任意位置的照片文件夹，以创新的浏览方式展示照片。

**主要功能**:
- TikTok风格的上下滑动浏览照片
- 支持添加任意位置的相册（本地、iCloud等）
- 相册分类和照片管理
- 可爱风格的iOS界面设计
- 浏览模式自定义（上下滑动/左右滑动）
- 图片查看、收藏功能

## 开发环境设置

### 前提条件

- Node.js (v14 或更高版本)
- pnpm (v10.5.2 或更高版本)

### 安装依赖

```bash
# 安装所有应用的依赖
pnpm i
```

#### 启动方式

你可以通过以下几种方式运行应用：

1. **直接启动特定应用**：
```bash
# 启动主页（端口3000）
pnpm start
```

3. **访问应用**：
   - 主页：http://localhost:3000

## 技术说明

- 各应用使用纯静态 HTML/CSS/JavaScript 开发
- 使用 `http-server` 包提供静态文件服务器
- 项目通过 pnpm 工作空间管理多个应用

## 项目管理

此项目使用 pnpm 工作空间来管理多个应用。每个应用都是独立的，但可以共享一些通用依赖。

### 添加新应用
在 `apps` 目录下创建新的应用目录

### 添加共享依赖

```bash
pnpm add -W <package-name>
```

## 贡献指南

欢迎为项目做出贡献：

1. Fork 本仓库
2. 创建您的特性分支 (`git checkout -b feature/amazing-feature`)
3. 提交您的更改 (`git commit -m 'Add some amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 开启一个 Pull Request

## 许可证

ISC 