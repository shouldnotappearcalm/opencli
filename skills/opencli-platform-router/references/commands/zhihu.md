# zhihu

Total commands: **4**

## Commands


### download
- Description: 导出知乎文章为 Markdown 格式
- Args:
  - `url` (required) — Article URL (zhuanlan.zhihu.com/p/xxx)
  - `output` (optional) — default='./zhihu-articles'; Output directory
  - `download-images` (optional) — type=boolean; default=false; Download images locally
- Example: `opencli zhihu download -f json`

### hot
- Description: 知乎热榜
- Args:
  - `limit` (optional) — type=int; default=20; Number of items to return
- Example: `opencli zhihu hot -f json`

### question
- Description: 知乎问题详情和回答
- Args:
  - `id` (required) — Question ID (numeric)
  - `limit` (optional) — type=int; default=5; Number of answers
- Example: `opencli zhihu question -f json`

### search
- Description: 知乎搜索
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=10; Number of results
- Example: `opencli zhihu search -f json`
