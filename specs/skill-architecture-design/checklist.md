# Checklist - 中高职教学管理36个Skill开发验收清单

## 开发规范检查

### 项目结构检查
- [x] 项目结构符合规范（skills/、specs/、README.md）
- [x] 目录命名规范（kebab-case）
- [x] README.md 包含完整项目说明

### 通用开发规范检查

#### 需求收集阶段
- [ ] 收集相关管理制度文件
- [ ] 梳理完整工作流程
- [ ] 确认表单清单
- [ ] 明确触发场景
- [ ] 与用户确认需求理解正确

#### 开发实现阶段
- [ ] SKILL.md 文件格式规范（YAML frontmatter + Markdown）
- [ ] 对话流程精简（3-7个核心问题）
- [ ] AI主动搜索填充机制已实现
- [ ] 模板文件完整
- [ ] 参考文档完整

#### 测试验证阶段
- [ ] 对话演示测试通过
- [ ] 用户确认效果满意
- [ ] 用户批准开发完成

#### 打包发布阶段
- [ ] 打包为 .zip 文件到 skills/ 目录
- [ ] 文件命名：`{skill-name}.zip`
- [ ] README.md 状态已更新
- [ ] checklist.md 验收状态已更新
- [ ] 已提交到Git仓库

---

## Phase 1: 基础建设（18个核心Skill）

### Skill 1: lark-vocational-talent-survey（专业人才需求调研）

**开发状态：✅ 已完成**

**开发规范检查**:
- [x] 需求收集完整（管理制度、工作流程、表单清单、触发场景）
- [x] 对话流程精简（7个核心问题）
- [x] AI主动搜索填充机制已实现
- [x] 用户确认需求
- [x] 用户批准方案
- [x] 测试演示通过
- [x] 用户批准完成
- [x] 打包为.zip文件
- [x] 状态同步完成

**功能验收**:
- [x] SKILL.md 文件完整
- [x] references/workflow.md 工作流程参考
- [x] references/industry-analysis-guide.md 行业分析指南
- [x] templates/survey-plan-template.md 调研方案模板

**工作流程自动化验收**:
- [x] 调研方案审批流程（9步）
- [x] 调研报告审核流程

**文档模板验收**:
- [x] 专业人才需求调研方案模板
- [x] 调研报告撰写体例

---

### Skill 2-18: 待开发

| ID | Skill名称 | 功能 | 开发规范检查 | 功能验收 |
|----|----------|------|-------------|---------|
| 2 | lark-vocational-major-application | 新专业申报备案 | ⬜ | ⬜ |
| 3 | lark-vocational-major-planning | 专业建设子规划 | ⬜ | ⬜ |
| 4 | lark-vocational-teaching-scheme | 专业教学实施方案 | ⬜ | ⬜ |
| 5 | lark-vocational-course-standard | 课程标准管理 | ⬜ | ⬜ |
| 6 | lark-vocational-major-evaluation | 专业建设评价 | ⬜ | ⬜ |
| 7 | lark-vocational-semester-plan | 部门学期工作计划 | ⬜ | ⬜ |
| 8 | lark-vocational-calendar | 校历编制 | ⬜ | ⬜ |
| 9 | lark-vocational-textbook | 教材选用与征订 | ⬜ | ⬜ |
| 10 | lark-vocational-course-adjustment | 调代课管理 | ⬜ | ⬜ |
| 11 | lark-vocational-teaching-plan | 授课计划管理 | ⬜ | ⬜ |
### Skill 12: lark-vocational-lesson-plan（教案管理）

**开发状态：✅ 已完成**

**功能验收**:
- [x] SKILL.md 文件完整
- [x] 精准/快速两种模式
- [x] 表格式/讲义式/提纲式三种教案形式
- [x] references/templates/ 教案模板完整
- [x] references/standards/ 设计原则完整
- [x] assets/templates/ 三种模板文件完整
- [x] references/examples/ 示例教案完整

---

### Skill 13-18: 待开发

| ID | Skill名称 | 功能 | 开发规范检查 | 功能验收 |
|----|----------|------|-------------|---------|
| 13 | lark-vocational-classroom-teaching | 课堂教学记录 | ⬜ | ⬜ |
| 14 | lark-vocational-homework | 作业批改管理 | ⬜ | ⬜ |
| 15 | lark-vocational-tutoring | 课外辅导答疑 | ⬜ | ⬜ |
| 16 | lark-vocational-teaching-log | 教学日志 | ⬜ | ⬜ |
| 17 | lark-vocational-practice-management | 实训实习管理 | ⬜ | ⬜ |
| 18 | lark-vocational-exam-management | 考务管理 | ⬜ | ⬜ |

---

## Phase 2: 扩展完善（18个扩展Skill）

| ID | Skill名称 | 功能 | 开发规范检查 | 功能验收 |
|----|----------|------|-------------|---------|
| 19 | lark-vocational-academic-meeting | 教务联席会议 | ⬜ | ⬜ |
| 20 | lark-vocational-supervision | 教学督导检查 | ⬜ | ⬜ |
| 21 | lark-vocational-classroom-observation | 听课评课 | ⬜ | ⬜ |
| 22 | lark-vocational-teaching-research | 教研活动 | ⬜ | ⬜ |
| 23 | lark-vocational-parent-meeting | 家长会 | ⬜ | ⬜ |
| 24 | lark-vocational-training-center | 实训中心管理 | ⬜ | ⬜ |
| 25 | lark-vocational-online-course | 网络课程管理 | ⬜ | ⬜ |
| 26 | lark-vocational-credit-management | 学分制管理 | ⬜ | ⬜ |
| 27 | lark-vocational-student-status | 学生学籍管理 | ⬜ | ⬜ |
| 28 | lark-vocational-teacher-planning | 师资队伍规划 | ⬜ | ⬜ |
| 29 | lark-vocational-teacher-training | 教师培养计划 | ⬜ | ⬜ |
| 30 | lark-vocational-teacher-evaluation | 教师考核评价 | ⬜ | ⬜ |
| 31 | lark-vocational-teacher-mentoring | 新教师带教 | ⬜ | ⬜ |
| 32 | lark-vocational-enterprise-practice | 企业实践锻炼 | ⬜ | ⬜ |
| 33 | lark-vocational-research-management | 科研课题管理 | ⬜ | ⬜ |
| 34 | lark-vocational-teacher-archive | 教师业务档案 | ⬜ | ⬜ |
| 35 | lark-vocational-library | 图书馆管理 | ⬜ | ⬜ |
| 36 | lark-vocational-classroom-booking | 教学场地借用 | ⬜ | ⬜ |

---

## 开发进度统计

| 阶段 | 总数 | 已完成 | 开发中 | 待开发 |
|------|------|--------|--------|--------|
| Phase 1 | 18 | 2 | 0 | 16 |
| Phase 2 | 18 | 0 | 0 | 18 |
| **总计** | **36** | **2** | **0** | **34** |

---

## 跨Skill集成验收

- [ ] 36个Skill可独立使用
- [ ] Skill之间数据可关联
- [ ] 统一的数据字典和编码规范
- [ ] 用户权限体系覆盖所有业务流程
- [ ] 完整的操作日志和审计追踪

---

## 文档与培训验收

- [ ] 每个Skill提供用户操作手册
- [ ] 每个Skill提供管理员配置指南
- [ ] 提供常见问题解答（FAQ）
- [ ] 完成至少一所学校的试点验证
- [ ] 收集试点反馈并完成优化

---

## 验收符号说明

| 符号 | 含义 |
|------|------|
| ✅ | 已完成并验收通过 |
| ⬜ | 待开发/待验收 |
| 🔄 | 开发中 |
