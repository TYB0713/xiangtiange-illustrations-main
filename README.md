README.md
复制 Skill 到 Codex skills 目录：

macOS / Linux:

mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./xiangtiange-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
Windows PowerShell:

New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.codex\skills"
Copy-Item -Recurse .\xiangtiange-illustrations "$env:USERPROFILE\.codex\skills\"
安装后重启 Codex 或开启新会话，让 Skill 重新加载。

使用
生成单张正文配图：

Use $xiangtiange-illustrations 为“产品开发流程：需求调研、竞品分析、方案设计、项目计划、开发跟踪、测试联调、验收上线发布”生成一张正文配图。
画面要怪诞但清爽，向天歌必须承担核心动作。
为文章规划配图：

Use $xiangtiange-illustrations 先不要生图。
请分析下面这篇文章哪里值得配图，输出 7 张左右的 shot list。
每张图写清楚：放在哪段后、主题、核心意思、结构类型、向天歌在做什么、建议中文标注词。

<粘贴文章>
生成一组 IP 样图：

Use $xiangtiange-illustrations 生成 8 张向天歌 IP 样图。
场景覆盖：历史教师、党建工作人员、UI 设计师、自媒体工作者、运营人员、架构师、AI 开发者。
每张单独生成，保持 16:9 横版、纯白背景、清爽手绘、向天歌承担核心动作。
目录结构
.
├── README.md
├── LICENSE
└── xiangtiange-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── assets/
    │   └── examples/
    │       ├── 00-xiangtiange-reference.png
    │       ├── 01-product-manager-prototype-review.png
    │       └── ...
    └── references/
        ├── xiangtiange-ip.md
        ├── style-dna.md
        ├── prompt-template.md
        ├── composition-patterns.md
        └── qa-checklist.md
真正需要安装到 Codex 的是子目录：

xiangtiange-illustrations/
示例图
示例图放在：

xiangtiange-illustrations/assets/examples/
它们覆盖：

历史教师：画原型、课堂讲解、学生管理
党建工作人员：安排学习、团队协作
测试人员：找 bug、测试用例、提交缺陷
UI 设计师：设计界面、调色、画图
自媒体工作者：拍摄、剪辑、文案、发布
运营人员：数据分析、活动策划、用户回复
架构师：系统架构、技术方案、评审
AI 开发者：训练模型、调参、数据处理
注意事项
图片里的中文越短越稳定。
向天歌必须参与核心动作，不能只是站在旁边。
如果角色关键特征丢失，比如一位清爽、干练、亲和的 IT 职场程序员。他有圆框眼镜、长头发、白色衬衫、黑色西裤和黑色皮鞋，建议重生成。
如果画面太像 PPT、课程页或复杂架构图，建议减少节点和文字。
示例图用于校准风格，不要直接复刻构图。
License
MIT License. See LICENSE.
