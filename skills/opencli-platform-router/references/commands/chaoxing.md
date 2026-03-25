# chaoxing

Total commands: **2**

## Commands


### assignments
- Description: 学习通作业列表
- Args:
  - `course` (optional) — type=string; 按课程名过滤（模糊匹配）
  - `status` (optional) — type=string; default='all'; 按状态过滤
  - `limit` (optional) — type=int; default=20; 最大返回数量
- Example: `opencli chaoxing assignments -f json`

### exams
- Description: 学习通考试列表
- Args:
  - `course` (optional) — type=string; 按课程名过滤（模糊匹配）
  - `status` (optional) — type=string; default='all'; 按状态过滤
  - `limit` (optional) — type=int; default=20; 最大返回数量
- Example: `opencli chaoxing exams -f json`
