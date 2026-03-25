# sinablog

Total commands: **4**

## Commands


### article
- Description: 获取新浪博客单篇文章详情
- Args:
  - `url` (required) — 文章URL（如 https://blog.sina.com.cn/s/blog_xxx.html）
- Example: `opencli sinablog article -f json`

### hot
- Description: 获取新浪博客热门文章/推荐
- Args:
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli sinablog hot -f json`

### search
- Description: 搜索新浪博客文章（通过新浪搜索）
- Args:
  - `keyword` (required) — 搜索关键词
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli sinablog search -f json`

### user
- Description: 获取新浪博客用户的文章列表
- Args:
  - `uid` (required) — 新浪博客用户ID（如 1234567890）
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli sinablog user -f json`
