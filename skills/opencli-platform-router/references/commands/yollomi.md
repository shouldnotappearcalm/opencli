# yollomi

Total commands: **12**

## Commands


### background
- Description: Generate AI background for a product/object image (5 credits)
- Args:
  - `image` (required) — Image URL (upload via
  - `prompt` (optional) — default=''; Background description (optional)
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi background -f json`

### edit
- Description: Edit images with AI text prompts (Qwen image edit)
- Args:
  - `image` (required) — Input image URL (upload via
  - `prompt` (required) — Editing instruction (e.g.
  - `model` (optional) — default='qwen-image-edit'; Edit model
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi edit -f json`

### face-swap
- Description: Swap faces between two photos (3 credits)
- Args:
  - `source` (required) — Source face image URL
  - `target` (required) — Target photo URL
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi face-swap -f json`

### generate
- Description: Generate images with AI (text-to-image or image-to-image)
- Args:
  - `prompt` (required) — Text prompt describing the image
  - `model` (optional) — default='z-image-turbo'; Model ID (z-image-turbo, flux-schnell, nano-banana, flux-2-pro, ...)
  - `ratio` (optional) — default='1:1'; Aspect ratio
  - `image` (optional) — Input image URL for image-to-image (upload via
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URLs, skip download
- Example: `opencli yollomi generate -f json`

### models
- Description: List available Yollomi AI models (image, video, tools)
- Args:
  - `type` (optional) — default='all'; Filter by model type
- Example: `opencli yollomi models -f json`

### object-remover
- Description: Remove unwanted objects from images (3 credits)
- Args:
  - `image` (required) — Image URL
  - `mask` (required) — Mask image URL (white = area to remove)
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi object-remover -f json`

### remove-bg
- Description: Remove image background with AI (free)
- Args:
  - `image` (required) — Image URL to remove background from
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi remove-bg -f json`

### restore
- Description: Restore old or damaged photos with AI (4 credits)
- Args:
  - `image` (required) — Image URL to restore
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi restore -f json`

### try-on
- Description: Virtual try-on — see how clothes look on a person (3 credits)
- Args:
  - `person` (required) — Person photo URL (upload via
  - `cloth` (required) — Clothing image URL
  - `cloth-type` (optional) — default='upper'; Clothing type
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi try-on -f json`

### upload
- Description: Upload an image or video to Yollomi (returns URL for other commands)
- Args:
  - `file` (required) — Local file path to upload
- Example: `opencli yollomi upload -f json`

### upscale
- Description: Upscale image resolution with AI (1 credit)
- Args:
  - `image` (required) — Image URL to upscale
  - `scale` (optional) — default='2'; Upscale factor (2 or 4)
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL
- Example: `opencli yollomi upscale -f json`

### video
- Description: Generate videos with AI (text-to-video or image-to-video)
- Args:
  - `prompt` (required) — Text prompt describing the video
  - `model` (optional) — default='kling-2-1'; Model (kling-2-1, openai-sora-2, google-veo-3-1, wan-2-5-t2v, ...)
  - `image` (optional) — Input image URL for image-to-video
  - `ratio` (optional) — default='16:9'; Aspect ratio
  - `output` (optional) — default='./yollomi-output'; Output directory
  - `no-download` (optional) — type=boolean; default=false; Only show URL, skip download
- Example: `opencli yollomi video -f json`
