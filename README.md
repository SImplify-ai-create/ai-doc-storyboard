# ai-doc-storyboard

**5 段式 AI 纪录片分镜设计** — 适配 TapNow/Sora/Veo 的"首帧+尾帧图生视频"工作流。

## 5 段式结构（顺序不变）

```
1. 核心主题      ← 3-6个风格标签，给AI定调子
2. 人物与基础设定 ← Who & 服装 & 场景
3. 氛围与画质     ← 摄影机型号+色调+风格参考
4. 运镜规则       ← 单镜头/角度/呼吸感
5. 分镜(时间轴)    ← 按镜展开：画面+首帧+尾帧+动作+镜头+旁白
```

## 段1·核心主题（标签公式）

```
画面类型 | 题材 | 美学风格 | 情绪 | 画质锚点
```

水墨史诗纪录片示例：
```
traditional Chinese ink painting style | wartime cultural heritage | crimson red and gold accents | epic solemn | cinematic film grain
```

## 段2-4·通用模板

| 段 | 内容 |
|----|------|
| 人物 | 面部特征+服装质地+表情基调（"杜绝美化，保留瑕疵"） |
| 场景 | 写动态环境（风/烟/雾/光），不出氛围 |
| 画质 | 摄影机型号（IMAX胶片/Panavision C系/索尼威尼斯）+色调（低饱和灰蓝/青橙/红金） |
| 运镜 | 景别+角度+运动+呼吸感（"如呼吸般的轻微镜头浮动"） |

## 段5·分镜表格式

| 项 | 内容 |
|----|------|
| 画面 | 全景/中景/特写 + 主体动作 |
| 首帧 | 静态起始状态描述 |
| 尾帧 | 动态终点状态描述 |
| 动作提示词 | 主体运动的英文描述 |
| 镜头语言 | 景别+运动+光影 |
| 情绪 | 该镜情绪基调 |
| 旁白 | 对应解说词 |

## 提示词公式（每镜必用）

```
【主体】+【动作/变化】+【环境】+【情绪/氛围】+【镜头语言】+【风格锚定】+【画质后缀】
```

## 风格锚定词（统一追加）

```
traditional Chinese ink painting style with crimson red and gold accents, epic cinematic atmosphere,
film grain texture, moody lighting, 16:9 aspect ratio, high detail, no text, no people faces clearly visible
```

## 镜长建议

- 每镜 8 秒，便于后续配乐节拍锁定（BPM = 60）
- 总镜数 = 总时长 ÷ 8
- 三幕比例约 5:12:5（序:征途:归来）

## 推荐模型

| 模型 | 时长 | 适用 |
|------|------|------|
| Sora 2 | 8-12s | 首选，时长够 |
| Veo 3.1 | 4-6s | 备选，多段拼接 |
| Kling 3.0 | 5-10s | 动作节奏强 |

## 三个反直觉原则

1. **不要给参考图，除非画质够高** — 垫图容易复现画风而非设计
2. **描述瑕疵 = 描述真实** — 磨损、战损、油污比"高质量"管用
3. **结尾留白** — 不堆特效，"只有身穿不完整战衣的人站在原地"

## 模板使用

打开 [`storyboard_template.md`](storyboard_template.md)，按 5 段式结构填写即可。

## 许可

MIT
