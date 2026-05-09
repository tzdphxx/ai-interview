# InterviewPilot

InterviewPilot 是一个个人 AI 面试练习项目，包含简历分析、模拟面试、语音面试、知识库问答和面试日程管理等功能。

## 项目功能

- 简历上传与 AI 分析
- 文本模拟面试与回答评估
- 语音模拟面试，支持 ASR / TTS
- 知识库上传与 RAG 问答
- 面试日程管理
- 多模型服务商配置

## 技术栈

- 后端：Java 21、Spring Boot 4、Spring AI、Gradle
- 前端：React 18、TypeScript、Vite
- 数据库：PostgreSQL、pgvector
- 缓存与队列：Redis
- 文件存储：MinIO 或其他 S3 兼容服务

## 本地运行

启动基础依赖：

```bash
docker compose -f docker-compose.dev.yml up -d
```

启动后端：

```bash
./gradlew :app:bootRun
```

启动前端：

```bash
cd frontend
pnpm install
pnpm dev
```

接口文档地址：

```text
http://localhost:8080/swagger-ui.html
```

## Docker 部署

```bash
docker compose up -d --build
```

## 说明

运行前需要自行配置 AI 服务商 API Key，例如 DashScope、Kimi、DeepSeek 或其他 OpenAI 兼容服务。

## 开源协议

本项目基于 AGPL-3.0 协议发布，详情见 `LICENSE` 和 `NOTICE`。
