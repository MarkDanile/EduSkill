# 中高职教学管理运行标准化体系 Skill 开发规划规范

## Why

贯彻落实《教育部关于深化职业教育教学改革全面提高人才培养质量的若干意见》（教职成[2015]6号）和《上海市教育委员会关于印发中等职业技术学校教学管理工作指导意见的通知》（沪教委职【2013】22号）文件精神，以"制度流程化,流程表单化,表单信息化"为理念，通过梳理学校教学管理架构（教学管理制度66个，工作流程73个，工作表单108个），形成行业范式，赋能各中高职院校的AI数字化转型。

## What Changes

将36个教学管理模块按业务领域划分为36个独立Skill，每个Skill对应一个核心业务模块。

## 项目结构

```
EduSkill/
├── skills/                              # AI技能目录
│   ├── lark-vocational-talent-survey/  # Skill 1
│   │   ├── SKILL.md
│   │   ├── references/                  # 参考文档
│   │   └── templates/                  # 文档模板
│   ├── lark-vocational-major-application/  # Skill 2
│   └── ...                              # 更多技能
│
├── specs/                               # 开发规范文档
│   └── skill-architecture-design/
│       ├── spec.md                      # 本文档
│       ├── tasks.md                     # 开发任务清单
│       └── checklist.md                 # 验收清单
│
└── README.md
```

---

## 📋 Skill 开发规范

### 开发流程

每个Skill的开发遵循以下标准流程：

```
┌─────────────────────────────────────────────────────────────────┐
│                     Skill 开发标准流程                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│  1️⃣ 需求收集    →    2️⃣ 方案确认    →    3️⃣ 开发实现         │
│  用户提供管理制度     问答确认需求            编写Skill文档         │
│  工作流程说明        用户批准方案            创建模板参考           │
│                                                                  │
│         ↓                                                        │
│                                                                  │
│  4️⃣ 测试验证    →    5️⃣ 打包发布    →    6️⃣ 提交代码         │
│  对话演示测试        打包为.zip文件          git commit push       │
│  用户确认效果        更新README状态                               │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

### 开发规则

#### 规则1: 开发前必须收集完整需求

在开始开发前，必须从用户处收集以下信息：

| 信息类型 | 内容 | 必须/可选 |
|----------|------|----------|
| 管理制度 | 相关管理制度文件 | 必须 |
| 工作流程 | 完整的业务流程步骤 | 必须 |
| 表单清单 | 涉及的表单/文档列表 | 必须 |
| 触发场景 | 何时使用此Skill | 必须 |

#### 规则2: 对话引导 + AI自动填充

**对话流程设计原则：**
- 精简核心问题（通常3-7个）
- 其他内容由AI主动搜索填充
- 允许用户跳过非关键信息

**AI主动填充内容：**
- 最新政策文件搜索
- 行业趋势分析
- 标准模板生成
- 专业特色内容补充

#### 规则3: 必须经过用户确认

每个Skill开发必须经过：
1. **需求确认** - 收集管理制度后，与用户确认理解是否正确
2. **方案确认** - 开始开发前，展示开发计划
3. **效果确认** - 测试演示后，获得用户批准

#### 规则4: 打包规范

每个Skill完成后必须：
1. 打包为 `.zip` 文件到 `skills/` 目录
2. 文件命名：`{skill-name}.zip`
3. 提交到Git仓库

#### 规则5: 状态同步

每次提交必须同步更新：
1. `README.md` 中的技能列表状态
2. `specs/skill-architecture-design/checklist.md` 中的验收状态

---

### SKILL.md 标准格式

```yaml
---
name: skill-name
description: 技能描述，包含触发场景（用户会说什么话触发此技能）
---

# 技能标题

## Overview
功能概述，2-3句话说明技能用途

## Workflow
### Step 1: [步骤名称]
具体流程说明

### Step 2: [步骤名称]
具体流程说明

## Resources
- `templates/` - 文档模板
- `references/` - 参考文档
```

### Skill 目录结构

```
skill-name/
├── SKILL.md              # 技能主文件（必需）
├── references/           # 参考文档（可选）
│   ├── workflow.md       # 工作流程参考
│   └── *.md             # 其他参考
├── templates/            # 文档模板（可选）
│   └── *.md             # 模板文件
└── scripts/             # 脚本文件（可选）
    └── *.py
```

---

## 36个Skill列表

### Phase 1: 基础建设（18个核心Skill）

| ID | Skill名称 | 功能 | 状态 |
|----|----------|------|------|
| 1 | lark-vocational-talent-survey | 专业人才需求调研 | ✅ 已完成 |
| 2 | lark-vocational-major-application | 新专业申报备案 | 📋 待开发 |
| 3 | lark-vocational-major-planning | 专业建设子规划 | 📋 待开发 |
| 4 | lark-vocational-teaching-scheme | 专业教学实施方案 | 📋 待开发 |
| 5 | lark-vocational-course-standard | 课程标准管理 | 📋 待开发 |
| 6 | lark-vocational-major-evaluation | 专业建设评价 | 📋 待开发 |
| 7 | lark-vocational-semester-plan | 部门学期工作计划 | 📋 待开发 |
| 8 | lark-vocational-calendar | 校历编制 | 📋 待开发 |
| 9 | lark-vocational-textbook | 教材选用与征订 | 📋 待开发 |
| 10 | lark-vocational-course-adjustment | 调代课管理 | 📋 待开发 |
| 11 | lark-vocational-teaching-plan | 授课计划管理 | 📋 待开发 |
| 12 | lark-vocational-lesson-plan | 教案管理 | 📋 待开发 |
| 13 | lark-vocational-classroom-teaching | 课堂教学记录 | 📋 待开发 |
| 14 | lark-vocational-homework | 作业批改管理 | 📋 待开发 |
| 15 | lark-vocational-tutoring | 课外辅导答疑 | 📋 待开发 |
| 16 | lark-vocational-teaching-log | 教学日志 | 📋 待开发 |
| 17 | lark-vocational-practice-management | 实训实习管理 | 📋 待开发 |
| 18 | lark-vocational-exam-management | 考务管理 | 📋 待开发 |

### Phase 2: 扩展完善（18个扩展Skill）

| ID | Skill名称 | 功能 | 状态 |
|----|----------|------|------|
| 19 | lark-vocational-academic-meeting | 教务联席会议 | 📋 待开发 |
| 20 | lark-vocational-supervision | 教学督导检查 | 📋 待开发 |
| 21 | lark-vocational-classroom-observation | 听课评课 | 📋 待开发 |
| 22 | lark-vocational-teaching-research | 教研活动 | 📋 待开发 |
| 23 | lark-vocational-parent-meeting | 家长会 | 📋 待开发 |
| 24 | lark-vocational-training-center | 实训中心管理 | 📋 待开发 |
| 25 | lark-vocational-online-course | 网络课程管理 | 📋 待开发 |
| 26 | lark-vocational-credit-management | 学分制管理 | 📋 待开发 |
| 27 | lark-vocational-student-status | 学生学籍管理 | 📋 待开发 |
| 28 | lark-vocational-teacher-planning | 师资队伍规划 | 📋 待开发 |
| 29 | lark-vocational-teacher-training | 教师培养计划 | 📋 待开发 |
| 30 | lark-vocational-teacher-evaluation | 教师考核评价 | 📋 待开发 |
| 31 | lark-vocational-teacher-mentoring | 新教师带教 | 📋 待开发 |
| 32 | lark-vocational-enterprise-practice | 企业实践锻炼 | 📋 待开发 |
| 33 | lark-vocational-research-management | 科研课题管理 | 📋 待开发 |
| 34 | lark-vocational-teacher-archive | 教师业务档案 | 📋 待开发 |
| 35 | lark-vocational-library | 图书馆管理 | 📋 待开发 |
| 36 | lark-vocational-classroom-booking | 教学场地借用 | 📋 待开发 |

---

## 开发进度统计

| 阶段 | 总数 | 已完成 | 待开发 |
|------|------|--------|--------|
| Phase 1 | 18 | 1 | 17 |
| Phase 2 | 18 | 0 | 18 |
| **总计** | **36** | **1** | **35** |

---

## 详细Skill设计

---

### Skill 1: lark-vocational-talent-survey（专业人才需求调研）

#### 功能定位
覆盖专业设置前的市场需求调研全流程，包括调研方案制定、调研实施、报告编制。

#### 核心表单清单
| 表单名称 | 功能描述 |
|---------|---------|
| 专业人才需求调研方案 | 调研对象、调研内容、调研周期设计 |
| 专业人才需求调研报告 | 调研结果汇总分析 |

#### 工作流程清单
- 专业人才需求调研流程

#### 触发场景
- 教务主任需要制定新专业设置前的市场调研

---

### Skill 2: lark-vocational-major-application（新专业申报备案）

#### 功能定位
覆盖新专业开设可行性论证与上海市新专业申报备案。

#### 核心表单清单
| 表单名称 | 功能描述 |
|---------|---------|
| 专业设置可行性分析报告 | 新专业开设可行性论证 |
| 新设专业备案表 | 上海市新专业申报 |
| 专业建设专家指导委员会活动记录 | 专家评审会议纪要 |

#### 工作流程清单
- 专业设置可行性分析流程

#### 触发场景
- 学校计划开设新专业需要申报备案

---

### Skill 3-36: （详见 tasks.md）

---

## 技术规范

### 多维表格建表规范
每个Skill下的业务模块需建立对应的多维表格，包含：
- 主数据表：存储核心业务数据
- 配置表：存储枚举选项、状态码等
- 日志表：记录数据变更历史

### 文档模板规范
每个Skill需提供标准文档模板：
- 管理制度的文档
- 工作表单的模板
- 流程图的可视化展示

## 验收标准

### 基础验收
- [x] 每个Skill包含完整的表单清单
- [x] 每个Skill覆盖对应的工作流程
- [x] 每个Skill提供操作指引文档

### 进阶验收
- [ ] 实现工作流程自动化（Workflow）
- [ ] 提供数据分析仪表盘（Dashboard）
- [ ] 支持批量数据导入导出
