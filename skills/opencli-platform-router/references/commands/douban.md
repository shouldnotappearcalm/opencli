# douban

Total commands: **7**

## Commands


### book-hot
- Description: 豆瓣图书热门榜单
- Args:
  - `limit` (optional) — type=int; default=20; 返回的图书数量
- Example: `opencli douban book-hot -f json`

### marks
- Description: 导出个人观影标记
- Args:
  - `status` (optional) — default='collect'; 标记类型: collect(看过), wish(想看), do(在看), all(全部)
  - `limit` (optional) — type=int; default=50; 导出数量， 0 表示全部
  - `uid` (optional) — 用户ID，不填则使用当前登录账号
- Example: `opencli douban marks -f json`

### movie-hot
- Description: 豆瓣电影热门榜单
- Args:
  - `limit` (optional) — type=int; default=20; 返回的电影数量
- Example: `opencli douban movie-hot -f json`

### reviews
- Description: 导出个人影评
- Args:
  - `limit` (optional) — type=int; default=20; 导出数量
  - `uid` (optional) — 用户ID，不填则使用当前登录账号
  - `full` (optional) — type=bool; default=false; 获取完整影评内容
- Example: `opencli douban reviews -f json`

### search
- Description: 搜索豆瓣电影、图书或音乐
- Args:
  - `type` (optional) — default='movie'; 搜索类型（movie=电影, book=图书, music=音乐）
  - `keyword` (required) — 搜索关键词
  - `limit` (optional) — type=int; default=20; 返回结果数量
- Example: `opencli douban search -f json`

### subject
- Description: 获取电影详情
- Args:
  - `id` (required) — type=str; 电影 ID
- Example: `opencli douban subject -f json`

### top250
- Description: 豆瓣电影 Top250
- Args:
  - `limit` (optional) — type=int; default=250; 返回结果数量
- Example: `opencli douban top250 -f json`
