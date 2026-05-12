# EduSkill
教育行业的 Skill 技能开发

## 36个中高职教学管理技能列表

| Skill ID | Skill名称 | 状态 | 说明 |
|----------|----------|------|------|
| 1 | edu-vocational-talent-survey | ✅ 已完成 | 专业人才需求调研方案编制与报告生成 |
| 2 | edu-vocational-feasibility-report | ✅ 已完成 | 专业设置可行性分析报告编制 |
| 3 | edu-vocational-major-planning | ⏳ 待开发 | 专业建设子规划编制与管理 |
| 4 | edu-vocational-teaching-scheme | ⏳ 待开发 | 专业教学实施方案（中高职贯通/三年制）编制 |
| 5 | edu-vocational-course-standard | ⏳ 待开发 | 课程标准审批与管理 |
| 6 | edu-vocational-major-evaluation | ⏳ 待开发 | 专业建设评价指标体系与考核 |
| 7 | edu-vocational-semester-plan | ⏳ 待开发 | 部门学期工作计划制定与审批 |
| 8 | edu-vocational-calendar | ⏳ 待开发 | 校历编制与教学进程表管理 |
| 9 | edu-vocational-textbook | ⏳ 待开发 | 教材选用、征订、发放与反馈 |
| 10 | edu-vocational-course-adjustment | ⏳ 待开发 | 调（代）课与停课申请管理 |
| 11 | edu-vocational-teaching-plan | ⏳ 待开发 | 课程授课计划制定与管理 |
| 12 | edu-vocational-lesson-plan | ✅ 已完成 | 教案编写、提交与审核 |
| 13 | edu-vocational-classroom-teaching | ⏳ 待开发 | 课堂教学记录与管理 |
| 14 | edu-vocational-homework | ⏳ 待开发 | 作业布置、批改与登记 |
| 15 | edu-vocational-tutoring | ⏳ 待开发 | 课外辅导与答疑安排记录 |
| 16 | edu-vocational-teaching-log | ⏳ 待开发 | 教学日志填写与审核 |
| 17 | edu-vocational-practice-management | ⏳ 待开发 | 实训教学、工学交替、顶岗实习管理 |
| 18 | edu-vocational-exam-management | ⏳ 待开发 | 试卷命题、监考、阅卷、成绩管理 |
| 19 | edu-vocational-academic-meeting | ⏳ 待开发 | 教务联席会议管理与记录 |
| 20 | edu-vocational-supervision | ⏳ 待开发 | 教学督导检查与事故处理 |
| 21 | edu-vocational-classroom-observation | ⏳ 待开发 | 听课评课安排与记录 |
| 22 | edu-vocational-teaching-research | ⏳ 待开发 | 教研活动申报与管理 |
| 23 | edu-vocational-parent-meeting | ⏳ 待开发 | 家长会组织与管理 |
| 24 | edu-vocational-training-center | ⏳ 待开发 | 实训中心设备与耗材管理 |
| 25 | edu-vocational-online-course | ⏳ 待开发 | 网络在线课程建设与开课管理 |
| 26 | edu-vocational-credit-management | ⏳ 待开发 | 学生学分认定与转换管理 |
| 27 | edu-vocational-student-status | ⏳ 待开发 | 学生学籍信息管理 |
| 28 | edu-vocational-teacher-planning | ⏳ 待开发 | 师资队伍规划编制 |
| 29 | edu-vocational-teacher-training | ⏳ 待开发 | 教师年度培养计划与个人发展规划 |
| 30 | edu-vocational-teacher-evaluation | ⏳ 待开发 | 教师多维度考核评价 |
| 31 | edu-vocational-teacher-mentoring | ⏳ 待开发 | 新教师带教与兼职教师聘任 |
| 32 | edu-vocational-enterprise-practice | ⏳ 待开发 | 教师企业实践锻炼管理 |
| 33 | edu-vocational-research-management | ⏳ 待开发 | 科研课题与成果评选管理 |
| 34 | edu-vocational-teacher-archive | ⏳ 待开发 | 教师业务档案管理 |
| 35 | edu-vocational-library | ⏳ 待开发 | 图书馆图书征订、借阅管理 |
| 36 | edu-vocational-classroom-booking | ⏳ 待开发 | 教学场地借用管理 |

## 项目结构

```
EduSkill/
├── skills/
│   ├── edu-vocational-talent-survey/
│   │   ├── SKILL.md
│   │   ├── references/
│   │   │   ├── workflow.md
│   │   │   └── industry-analysis-guide.md
│   │   └── templates/
│   │       └── survey-plan-template.md
│   ├── edu-vocational-talent-survey.zip
│   ├── edu-vocational-feasibility-report/
│   │   ├── SKILL.md
│   │   ├── references/
│   │   │   ├── workflow.md
│   │   │   └── policy-guide.md
│   │   └── templates/
│   │       └── feasibility-report-template.md
│   ├── edu-vocational-feasibility-report.zip
│   ├── edu-vocational-lesson-plan/
│   │   ├── SKILL.md
│   │   ├── CHANGELOG.md
│   │   ├── SKILL-DEVELOPMENT-GUIDE.md
│   │   ├── assets/
│   │   │   └── templates/
│   │   │       ├── lecture-template.md
│   │   │       ├── outline-template.md
│   │   │       └── table-template.md
│   │   ├── docs/
│   │   │   └── prompts-for-deployment.md
│   │   └── references/
│   │       ├── examples/
│   │       │   ├── professional-course-example.md
│   │       │   └── public-course-example.md
│   │       ├── standards/
│   │       │   └── design-principles.md
│   │       └── templates/
│   │           ├── acceptance-checklist.md
│   │           ├── deployment-guide-template.md
│   │           ├── reflection-template.md
│   │           ├── system-prompt-template.md
│   │           ├── teaching-analysis.md
│   │           ├── teaching-process.md
│   │           └── user-trigger-template.md
│   ├── edu-vocational-lesson-plan.zip
│   └── ... (其他33个技能待开发)
└── README.md
```

## 使用说明

### 导入技能到 Coze 平台

1. 从 `skills/` 目录下载所需技能的 `.zip` 文件
2. 登录 Coze 平台，进入个人空间或团队空间
3. 点击「创建 Bot」→「导入技能」
4. 选择下载的 `.zip` 文件并上传
5. 根据平台指引完成技能配置

### 技能开发规范

- 每个技能独立打包为 `.zip` 文件
- 遵循统一的目录结构：`SKILL.md` + `references/` + `templates/`
- AI 自动搜索最新政策、行业数据和标准
- 通过对话引导用户完成核心信息收集

## 开发进度

- ✅ 已完成: 3/36
- ⏳ 待开发: 33/36
