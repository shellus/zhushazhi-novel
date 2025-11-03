# 朱砂痣

> 基于 Docsify 的在线小说阅读网站

## 项目简介

这是一个都市奇幻小说《朱砂痣》的在线阅读平台,采用 Docsify 构建的纯静态网站,支持章节导航、全文搜索、深色模式等功能。

## 技术选型

- **前端框架**: [Docsify](https://docsify.js.org/) - 轻量级文档网站生成器
- **主题**: Docsify Themeable - 支持自定义主题和深色模式
- **插件**:
  - docsify-search - 全文搜索功能
  - docsify-pagination - 章节分页导航
- **部署**: Docker + Nginx

## 项目结构

```
.
├── README.md              # 项目技术文档(本文件)
├── Dockerfile             # Docker镜像构建文件
├── docker-compose.yml     # Docker Compose配置
├── .gitignore
└── web/                   # 网站根目录(Docsify工作目录)
    ├── README.md          # 网站首页(小说介绍)
    ├── index.html         # Docsify配置
    ├── _sidebar.md        # 侧边栏导航
    ├── 朱砂痣-小说大纲.md  # 小说创作大纲
    └── chapters/          # 章节目录
        ├── chapter-01.md
        ├── chapter-02.md
        └── ...
```

## 快速开始

### 开发模式

使用 Docsify CLI 启动本地开发服务器,支持热重载:

```bash
# 安装 docsify-cli(仅需安装一次)
npm i -g docsify-cli

# 启动开发服务器
docsify serve web

# 默认访问 http://localhost:3000
```

修改 Markdown 文件后会自动刷新浏览器,无需手动重新加载。

### 生产部署

使用 Docker Compose 一键启动:

```bash
# 启动服务
docker-compose up -d

# 停止服务
docker-compose down

# 查看日志
docker-compose logs -f
```

访问 http://localhost:8888

## 创作进度

- ✅ 第1章:朱砂痣的秘密(2847字)
- ✅ 第2章:校园怪谈(3124字)
- ✅ 第3章:神秘的男人(3287字)
- ✅ 第4章:镇魂针发烫(3186字)

**总进度:** 12444 / 200000 字(约6.2%)
