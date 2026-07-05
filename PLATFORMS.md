# 跨平台适配指南

本文件详细说明如何在OpenClaw、Hermes、Codex、ChatGPT、Claude等平台使用"前进写作引擎"。

---

## 快速开始（3步）

### Step 1：获取System Prompt

- 中文使用：打开 `prompts/system-prompt-zh.md`，全选复制
- 英文使用：打开 `prompts/system-prompt-en.md`，全选复制

### Step 2：粘贴到目标平台

| 平台 | 粘贴位置 |
|------|----------|
| **OpenClaw** | Expert → System Prompt |
| **Hermes** | 角色设定 / System Prompt |
| **Codex / ChatGPT** | System Message / Instructions |
| **Claude** | Project Instructions / System Prompt |
| **通义千问** | 系统指令 |
| **文心一言** | 系统指令 / 角色设定 |
| **混元** | 系统指令 |
| **DeepSeek** | System Prompt |

### Step 3：开始写作

输入示例：
- "帮我写一篇关于AI对就业影响的公众号文章"
- "写一个小红书文案，推荐一款效率工具"
- "写一篇抖音视频脚本，讲职场沟通"
- "用我的风格写一篇关于新零售的行业分析"

---

## 各平台详细适配

### OpenClaw

1. 创建新Expert
2. 名称填：`前进写作引擎`
3. System Prompt粘贴 `system-prompt-zh.md` 全部内容
4. 温度建议：0.7-0.8（创造性写作需要一定随机性）
5. 最大token：4096（长文写作需要足够空间）

### Hermes

1. 创建新角色
2. 角色设定粘贴System Prompt
3. 对话模式选择"创作"或"专业"
4. 建议开启"联网搜索"功能（写作时获取最新素材）

### ChatGPT / Codex

1. 创建新GPT或打开Custom Instructions
2. Instructions粘贴System Prompt
3. 建议开启Web Search（获取最新案例和数据）
4. 如创建GPT：上传 `references/` 目录下的4个文件作为知识库

### Claude

1. 创建新Project
2. Project Instructions粘贴System Prompt
3. 上传 `references/` 目录下的文件作为参考文档
4. Claude的长文写作能力较强，适合公众号长文和深度分析

### 通义千问 / 文心一言 / 混元 / DeepSeek

1. 找到"系统指令"或"角色设定"入口
2. 粘贴System Prompt
3. 部分平台可能限制System Prompt长度，如超长可精简保留核心规则

---

## 参考文件说明

上传到平台知识库时可选择性使用以下文件：

| 文件 | 内容 | 是否必须 |
|------|------|----------|
| `references/writing-style-dna.md` | 用户写作风格DNA深度分析 | ✅ 推荐 |
| `references/viral-structures.md` | 爆款文案结构库（5平台×多类型） | ✅ 推荐 |
| `references/golden-quotes.md` | 金句库与生成公式 | ⬜ 可选 |
| `references/evolution-log.md` | 进化日志 | ⬜ 可选 |

---

## 使用技巧

### 1. 获取最佳效果

- **明确平台**："帮我写一篇**小红书**文案"比"帮我写个文案"效果好
- **明确类型**："写一篇**行业分析**"比"写篇文章"效果好
- **给参考**："参考我之前写新零售那篇的风格"效果更好
- **给数据**：提供你的数据/案例，AI会更好地融入

### 2. 触发自主进化

- "这篇不够犀利，参考我的风格重新优化"
- "分析我的写作风格，更新你的理解"
- "这篇金句不够多，加几个"
- "这个开头太平了，换个更有冲击力的"

### 3. 分平台调整

- **公众号**：直接说"写公众号文章"，AI会自动2500-5000字+小标题
- **小红书**：直接说"写小红书文案"，AI会自动500-1500字+emoji分段
- **抖音**：直接说"写抖音脚本"，AI会自动200-800字+前3秒钩子
