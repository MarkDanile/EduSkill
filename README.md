# EduSkill - 中高职教学管理AI数字化技能平台

> 中高职教学管理AI数字化转型解决方案

## 📋 项目简介

EduSkill 是一个面向中高职院校教学管理AI数字化的技能开发项目，通过模块化的Skill设计，将传统的教学管理业务（如人才需求调研、专业申报、考务管理等）转化为可智能执行的AI技能，提升教务工作效率。

### 核心理念

- **制度流程化** → 梳理教学管理制度，建立标准化工作流程
- **流程表单化** → 将流程转化为可操作的表单和审批节点
- **表单信息化** → 通过AI技能实现智能填写、自动生成、数据分析

### 项目目标

开发 **36个** 覆盖中高职教学管理全流程的AI技能，赋能各院校的AI数字化转型。

## 🏗️ 项目架构

```
EduSkill/
├── skills/                              # AI技能目录
│   ├── lark-vocational-talent-survey/   # 技能1：人才需求调研
│   │   ├── SKILL.md
│   │   ├── references/                   # 参考文档
│   │   └── templates/                    # 文档模板
│   └── ...                               # 更多技能
│
├── specs/                                # 开发规范文档
│   └── skill-architecture-design/
│       ├── spec.md                       # 技能设计规范
│       ├── tasks.md                      # 开发任务清单
│       └── checklist.md                  # 验收清单
│
└── README.md
```

## 📦 已发布技能

### 1. lark-vocational-talent-survey（专业人才需求调研）

**功能：** 通过对话引导+AI搜索，自动生成专业人才需求调研方案和报告

**适用场景：**
- 教务主任/专业带头人制定调研方案
- 专业设置前的可行性论证
- 年度人才需求调研

**核心流程：**
```
用户回答核心问题 → AI自动搜索政策/行业数据 → AI自动填充各章节 → 生成文档
```

**文件位置：** `skills/lark-vocational-talent-survey/`

**下载包：** `skills/lark-vocational-talent-survey.zip`

---

## 🚀 快速开始

### 在本项目中使用技能

1. **克隆项目**
```bash
git clone https://github.com/MarkDanile/EduSkill.git
cd EduSkill
```

2. **查看已发布的技能**
```bash
ls -la skills/
```

3. **查看技能详情**
```bash
cat skills/lark-vocational-talent-survey/SKILL.md
```

### 下载技能包

每个技能已打包为 `.zip` 文件，可直接下载使用：

```bash
ls -la skills/*.zip
```

---

## 📚 技能开发规范

### 开发流程

按照 [skill-creator](https://github.com/MarkDanile/EduSkill/blob/main/specs/skill-architecture-design/spec.md) 规范开发：

```
1. 收集管理制度 → 梳理工作流程
2. 初始化技能框架 → 创建技能目录结构
3. 编写技能文档 → 实现对话逻辑
4. 测试验证 → 打包发布
```

### 技能结构规范

```
skill-name/
├── SKILL.md              # 技能主文件（必需）
├── references/           # 参考文档（可选）
│   ├── workflow.md       # 工作流程参考
│   └── *.md
├── templates/            # 文档模板（可选）
│   └── *.md
└── scripts/             # 脚本文件（可选）
    └── *.py
```

### SKILL.md 格式要求

```yaml
---
name: skill-name
description: 技能描述，触发场景
---

# 技能标题

## Overview
功能概述

## Workflow
工作流程

## Resources
资源文件引用
```

---

## 🔄 导出到其他平台

### Coze 平台导出

Coze 支持通过 Bot 对话形式使用技能。导出步骤：

#### 步骤1：准备技能文档

将技能目录下的文件转换为 Coze 格式：

| 原始格式 | Coze 格式 |
|----------|-----------|
| `SKILL.md` | 技能说明（人设） |
| `workflow.md` | 对话流程提示词 |
| `templates/` | 预设模板 |
| `references/` | 知识库文档 |

#### 步骤2：创建 Coze Bot

1. 登录 [Coze](https://www.coze.cn/) 平台
2. 点击「创建 Bot」
3. 填写 Bot 信息：
   - **名称**：与技能名称一致
   - **描述**：技能功能描述
   - **人设与开场白**：从 `SKILL.md` 的 description 和 overview 提取

#### 步骤3：配置技能提示词

在 Coze Bot 的「技能配置」中，粘贴以下格式的提示词：

```
## 角色定位
你是一个[技能名称]，用于[功能描述]。

## 核心能力
1. [能力1]
2. [能力2]
3. [能力3]

## 对话流程
### Step 1: [步骤名称]
[具体流程]

### Step 2: [步骤名称]
[具体流程]

## 输出格式
[期望的输出格式]

## 参考资料
请参考以下文件：
- [文件名1]
- [文件名2]
```

#### 步骤4：导入知识库（如有）

如有 `references/` 目录下的文档：

1. 在 Coze Bot 中创建「知识库」
2. 上传参考文档
3. 关联知识库到 Bot

#### 步骤5：测试与发布

1. 在 Coze 平台测试对话
2. 调整提示词优化效果
3. 发布到 Coze 应用商店（可选）

---

### 其他平台导出参考

#### 通用导出格式

无论导出到哪个平台，都需要准备以下内容：

| 内容 | 说明 |
|------|------|
| **技能说明** | SKILL.md 的 description |
| **功能概述** | SKILL.md 的 overview |
| **对话流程** | SKILL.md 的 workflow |
| **输出模板** | templates/ 目录下的文件 |
| **参考文档** | references/ 目录下的文件 |

#### 提示词转换模板

将 Skill 的 `workflow` 转换为平台特定的提示词格式：

```markdown
# Role: [技能名称]

# Profile
- Language: 中文
- Description: [功能描述]

# Skills
## Skill 1: [子技能名称]
[具体实现]

## Skill 2: [子技能名称]
[具体实现]

# Workflow
[详细的工作流程]

# Output Format
[输出格式要求]
```

---

## 📖 技能列表（规划中）

### Phase 1: 基础建设（18个核心Skill）

| 编号 | 技能名称 | 功能 | 状态 |
|------|----------|------|------|
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
| 12 | lark-vocational-lesson-plan | 教案管理 | ✅ 已完成 |
| 13 | lark-vocational-classroom-teaching | 课堂教学记录 | 📋 待开发 |
| 14 | lark-vocational-homework | 作业批改管理 | 📋 待开发 |
| 15 | lark-vocational-tutoring | 课外辅导答疑 | 📋 待开发 |
| 16 | lark-vocational-teaching-log | 教学日志 | 📋 待开发 |
| 17 | lark-vocational-practice-management | 实训实习管理 | 📋 待开发 |
| 18 | lark-vocational-exam-management | 考务管理 | 📋 待开发 |
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

### 开发进度统计

| 阶段 | 总数 | 已完成 | 待开发 |
|------|------|--------|--------|
| Phase 1（基础建设） | 18 | 1 | 17 |
| Phase 2（扩展完善） | 18 | 0 | 18 |
| **总计** | **36** | **1** | **35** |

---

## 🛠️ 开发工具

### 技能打包工具

使用 `skill-creator` 提供的脚本打包技能：

```bash
# 初始化新技能
python3 scripts/init_skill.py <skill-name> --path <output-path>

# 打包技能为 zip
python3 scripts/package_skill.py <skill-folder> --output-dir <output-dir>
```

### 技能验证工具

```bash
# 验证技能结构
python3 scripts/validate_skill.py <skill-folder>
```

---

## 📝 贡献指南

### 提交新技能

1. Fork 本项目
2. 创建分支：`git checkout -b feature/new-skill`
3. 按照规范开发技能
4. 测试验证
5. 提交 Pull Request

### 技能开发检查清单

- [ ] SKILL.md 文件完整
- [ ] 对话流程符合规范
- [ ] 模板文件格式正确
- [ ] 通过打包验证
- [ ] 测试对话通过
- [ ] 打包为 .zip 文件

---

## 📄 许可证

本项目采用 MIT 许可证。

---

## 📞 联系方式

- **项目维护**：MarkDanile
- **GitHub**：[https://github.com/MarkDanile/EduSkill](https://github.com/MarkDanile/EduSkill)

---

## 🔗 相关资源

- [skill-creator 技能开发规范](https://github.com/MarkDanile/EduSkill/blob/main/specs/skill-architecture-design/spec.md)
- [Coze 平台](https://www.coze.cn/)
