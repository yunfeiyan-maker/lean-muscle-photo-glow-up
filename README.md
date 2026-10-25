![Lean Muscle Photo Glow-Up · 薄肌感男生修图 Skill](docs/assets/brand/lean-muscle-photo-glow-up-cover.png)

# 薄肌感男生修图 Skill

**Lean Muscle Photo Glow-Up**

为男生日常照、健身照和穿搭照提供可执行的 AI 修图规则。协调胸肩臂、腰胯与可见腿部的健体比例，通过肌肉形态对比形成运动感与视觉显高；自然改善面部状态，保留本人特征、真实肤质和原片自然色彩。

**规则版本 2.0.1** · **Markdown Agent Skill** · **16 组前后对照**

[快速开始](#快速开始) · [案例展示](docs/CASES.md) · [完整规则](skills/athletic-male-photo-retouch/SKILL.md) · [提示词](docs/prompts.md) · [更新记录](CHANGELOG.md)

默认整体约 **20%**、手臂约 **15%** 的综合视觉增强。手臂优先提升肩臂、二头肌与三头肌交界的自然分离度，按需要少量增加饱满度；原臂围足够时保留轮廓。百分比是视觉目标，不代表臂围加粗比例，用户本图明确要求优先。

## 适合什么照片

| 场景 | 处理重点 |
| --- | --- |
| 日常与旅行 | 自然面部状态、协调比例，以及与现场光线一致的肤质与肌肉明暗 |
| 健身与运动 | 胸肩背臂与上下身肌肉量协调，肩头饱满但不自动加粗手臂，保留自然曲面 |
| 泳裤、短裤与可见下肢 | 股四头肌外抛—膝部收束、腰胯—腿肌关系、可见人鱼线、小腿肌腹—踝部对比；保留原腿长与遮挡 |
| 穿搭与通勤 | 肩胸撑衣、衣料张力与真实褶皱，保留款式、接缝和标志 |

每张照片按可见部位、原片基础和明确需求单独处理。目标是更有训练感、状态更好的本人；不机械放大肌肉，不用极端腹肌分离、油亮或磨皮制造效果。

## 快速开始

### 1. 安装 Skill

[下载项目 ZIP](https://github.com/yunfeiyan-maker/lean-muscle-photo-glow-up/archive/refs/heads/main.zip)，将 `skills/athletic-male-photo-retouch/` 整个文件夹复制到：

- 项目内使用：`.agents/skills/`
- 个人使用：`~/.agents/skills/`

保留完整目录结构，并检查当前助手能否识别该 Skill。界面名称为 **薄肌感男生修图 Skill**；已有技术标识 `athletic-male-photo-retouch` 继续沿用。

```text
athletic-male-photo-retouch/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── 运动男子健体修图参考/
    ├── 面部与真实摄影标准.md
    └── 肌肉审美与形体调整规则.md
```

### 2. 上传照片并提出要求

> 使用 $athletic-male-photo-retouch 修这张照片。自然改善面部状态，协调胸肩臂与可见腰胯腿部的健体比例，保留本人五官、表情、真实皮肤、原片光线和自然色彩。根据这张照片选择适度增强，不做夸张增肌。请直接编辑并输出成片。

可补充“只调整肩胸比例”“腹肌不要明显”“保留背景与构图”等本图要求。同图返修请提供要继续使用的版本，并说明具体需要改动的位置。

### 3. 检查与返修

对照原图分别查看本人辨识度、肌群与腰胯腿比例、肤质光影、自然色彩及衣物细节；裁剪后按相近人物显示尺寸比较。若有问题，按照片编号说明具体区域；保留满意的部分，只返修需要调整的位置。

实际编辑需要当前助手提供可用的图像工具。本项目提供规则与参考，不包含模型、API 密钥或生成额度。

## 案例

| 案例1 原图 | 案例1 修图后 | 案例2 原图 | 案例2 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例1-前.jpg" alt="案例1原图" width="180"> | <img src="docs/assets/案例参考/案例1-后.jpg" alt="案例1修图后" width="180"> | <img src="docs/assets/案例参考/案例2-前.jpg" alt="案例2原图" width="180"> | <img src="docs/assets/案例参考/案例2-后.jpg" alt="案例2修图后" width="180"> |

| 案例3 原图 | 案例3 修图后 | 案例4 原图 | 案例4 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例3-前.jpg" alt="案例3原图" width="180"> | <img src="docs/assets/案例参考/案例3-后.jpg" alt="案例3修图后" width="180"> | <img src="docs/assets/案例参考/案例4-前.jpg" alt="案例4原图" width="180"> | <img src="docs/assets/案例参考/案例4-后.jpg" alt="案例4修图后" width="180"> |

| 案例5 原图 | 案例5 修图后 | 案例6 原图 | 案例6 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例5-前.jpg" alt="案例5原图" width="180"> | <img src="docs/assets/案例参考/案例5-后.jpg" alt="案例5修图后" width="180"> | <img src="docs/assets/案例参考/案例6-前.jpg" alt="案例6原图" width="180"> | <img src="docs/assets/案例参考/案例6-后.jpg" alt="案例6修图后" width="180"> |

| 案例7 原图 | 案例7 修图后 | 案例8 原图 | 案例8 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例7-前.jpg" alt="案例7原图" width="180"> | <img src="docs/assets/案例参考/案例7-后.jpg" alt="案例7修图后" width="180"> | <img src="docs/assets/案例参考/案例8-前.jpg" alt="案例8原图" width="180"> | <img src="docs/assets/案例参考/案例8-后.jpg" alt="案例8修图后" width="180"> |

| 案例9 原图 | 案例9 修图后 | 案例10 原图 | 案例10 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例9-前.jpg" alt="案例9原图" width="180"> | <img src="docs/assets/案例参考/案例9-后.jpg" alt="案例9修图后" width="180"> | <img src="docs/assets/案例参考/案例10-前.jpg" alt="案例10原图" width="180"> | <img src="docs/assets/案例参考/案例10-后.jpg" alt="案例10修图后" width="180"> |

| 案例11 原图 | 案例11 修图后 | 案例12 原图 | 案例12 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例11-前.jpg" alt="案例11原图" width="180"> | <img src="docs/assets/案例参考/案例11-后.jpg" alt="案例11修图后" width="180"> | <img src="docs/assets/案例参考/案例12-前.jpg" alt="案例12原图" width="180"> | <img src="docs/assets/案例参考/案例12-后.jpg" alt="案例12修图后" width="180"> |

| 案例13 原图 | 案例13 修图后 | 案例14 原图 | 案例14 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例13-前.jpg" alt="案例13原图" width="180"> | <img src="docs/assets/案例参考/案例13-后.jpg" alt="案例13修图后" width="180"> | <img src="docs/assets/案例参考/案例14-前.jpg" alt="案例14原图" width="180"> | <img src="docs/assets/案例参考/案例14-后.jpg" alt="案例14修图后" width="180"> |

| 案例15 原图 | 案例15 修图后 | 案例16 原图 | 案例16 修图后 |
| --- | --- | --- | --- |
| <img src="docs/assets/案例参考/案例15-前.jpg" alt="案例15原图" width="180"> | <img src="docs/assets/案例参考/案例15-后.jpg" alt="案例15修图后" width="180"> | <img src="docs/assets/案例参考/案例16-前.jpg" alt="案例16原图" width="180"> | <img src="docs/assets/案例参考/案例16-后.jpg" alt="案例16修图后" width="180"> |

[查看独立案例页与图片来源](docs/CASES.md)

## 规则与资源

| 文档 | 用途 |
| --- | --- |
| [Skill 主入口](skills/athletic-male-photo-retouch/SKILL.md) | 确定范围、制定目标、执行编辑、对照验收与必要返修 |
| [面部与真实摄影标准](skills/athletic-male-photo-retouch/运动男子健体修图参考/面部与真实摄影标准.md) | 本人特征、自然面部美化、肤质、光照与原片成像 |
| [肌肉审美与形体调整规则](skills/athletic-male-photo-retouch/运动男子健体修图参考/肌肉审美与形体调整规则.md) | 五维判断、肌群方向、比例、角度与衣料联动 |
| [提示词与返修示例](docs/prompts.md) | 未安装时的完整指令，以及局部修改的表达方式 |
| [更新记录](CHANGELOG.md) | 规则版本与项目维护记录 |
| [飞书教程](https://my.feishu.cn/wiki/QJ2Ywr3pLiPMx9kUX7QcGOK8nSe) | 补充教程；规则以本仓库当前文件为准 |

## 验证与使用说明

2.0.1 将本地手臂回调策略合入线上现有规则：整体约20%、手臂约15%，手臂分离度优先，并补充过粗与阴影过硬的验收。此次为规则与文档更新，完成静态校验，未新增出图验证。

1.5.0 补充运动员式腿形、腰胯比例、肤质保护与自然色彩分项验收。单张照片迭代中的形体方向获用户认可，但颜色饱和度仍需改进；本次自然色彩补充完成文档校验，尚未另行出图验证，也不能验证被遮挡的全腿比例。该次规则发布未新增私人测试照片；后续新增案例的来源见案例页。

此前 1.4.0 已完成规则与引用静态检查，以及本地三张照片的单轮版本对照。案例用于观察实际效果；有限样本不能证明所有人物、场景与工具具有相同表现，也不作为首轮成功率或版本优劣的统计证据。

生成式编辑仍可能改变面部细节、服装小字、镜像或背景，成片须逐张核对。当前未附开源许可证；案例图片仅用于经用户指定的展示，仓库公开不等于授予图片任意使用许可。
