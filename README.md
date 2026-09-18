
## 🚀 快速开始

### 环境要求

| 环境 | 版本要求 |
|:---|:---|
| JDK | 17 或 21 |
| MySQL | 5.7+ 或 8.0+ |
| Redis | 5.0+ |
| Node.js | 18+ |
| Maven | 3.9+ |
| Nacos | 2.x |

### 一键启动

```bash
# 1. 克隆项目
git clone https://github.com/your-org/ruoyi-office.git

# 2. 导入数据库
mysql -u root -p < sql/mysql/ruoyi-vue-pro.sql

# 3. 启动后端（先启动 Nacos）
cd ruoyi-office
mvn clean install -DskipTests
java -jar yudao-server/target/yudao-server.jar

# 4. 启动前端
cd ruoyi-office-vben
pnpm install
npm run dev:antd
```
---

## 📐 项目结构

### 后端模块

| 模块 | 说明 |
|:---|:---|
| `yudao-dependencies` | Maven 依赖版本管理 |
| `yudao-framework` | Java 框架核心拓展 |
| `yudao-gateway` | Spring Cloud 微服务网关 |
| `yudao-server` | 管理后台 + 用户 APP 服务端 |
| `yudao-module-system` | 系统管理（用户/角色/权限/租户） |
| `yudao-module-infra` | 基础设施（代码生成/文件/日志） |
| `yudao-module-bpm` | 工作流程引擎 |
| `yudao-module-oa` | OA 协同办公 |
| `yudao-module-hrm` | HRM 人力资源管理 |
| `yudao-module-crm` | CRM 客户关系管理 |
| `yudao-module-erp` | ERP 进销存管理 |
| `yudao-module-asset` | EAM 资产管理 |
| `yudao-module-wms` | WMS 仓储管理 |
| `yudao-module-mall` | MALL 企业商城 |
| `yudao-module-pay` | 支付系统 |
| `yudao-module-ai` | AI 大模型 |
| `yudao-module-iot` | IoT 物联网 |
| `yudao-module-member` | 会员中心 |
| `yudao-module-mp` | 微信公众号 |
| `yudao-module-report` | 数据报表 |

---