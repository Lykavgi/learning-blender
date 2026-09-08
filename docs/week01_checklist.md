# Week 01 Checklist — learning-blender

目的：把 Day0 到 Day7 的逐日操作清单写成一个可执行的 checklist，所有参考教材与示例文件均来自 GitHub。你可以直接在仓库按每项执行并在完成后把文件/图片提交到 projects/week01/ 下。

前置条件（完成一次性准备）
- 本地已安装：Blender、Git。推荐安装 VS Code。
- 已在 GitHub 创建仓库：`Lykavgi/learning-blender` 并已 clone 到本地。
- 必要的参考教程（下面会要求你打开这些 GitHub 页面并下载/使用它们的文件）：
  - Donut 示例（.blend 演示文件）：https://github.com/thecrazymage/Blender-Donut-Tutorial
  - 系列文字课程笔记（分课顺序步骤）：https://github.com/Mark-McCormack/Blender-Course-Notes
  - 学习笔记与速查（快捷键/技巧）：https://github.com/TristanCacqueray/learn-blender

文件位置（在你的仓库中保存成果）
- 项目文件夹：`projects/week01/`
- 日志/笔记：`notes/daily_log.md`
- 本清单（当前文件）：`docs/week01_checklist.md`

Day0 — 一次性准备（在 GitHub 要打开的页面与按键）
- 在浏览器打开并确认你的仓库首页：
  - 打开：https://github.com/Lykavgi/learning-blender
  - 界面要点：确认右上有 "Code" 绿色按钮（用于复制 clone 链接），左侧能看到文件树。
- 打开并 Star / Fork 三个参考仓库（在每个仓库页面右上角点击 Star 与 Fork）：
  - https://github.com/thecrazymage/Blender-Donut-Tutorial (点 Star / Fork)
  - https://github.com/Mark-McCormack/Blender-Course-Notes (点 Star / Fork)
  - https://github.com/TristanCacqueray/learn-blender (点 Star / Fork)
- 本地命令（在你的仓库根目录执行）：
  - mkdir -p projects/week01 notes resources docs
  - git add . && git commit -m "init learning-blender structure" && git push

Day1 — Donut lesson1（打开 GitHub 页面 / 本地操作）
- 在浏览器打开：
  - https://github.com/thecrazymage/Blender-Donut-Tutorial
  - 在仓库文件列表里找到 lesson1 或编号最小的 .blend 文件，点击文件名进入文件详情页，右上点击 "Download" 或在文件预览页点 "Raw" 下载
- 本地：
  - git checkout -b week01-day01
  - 在 Blender 中打开下载的 lesson1.blend（或教程指定文件），观察场景结构（Objects / Outliner / Camera / Light）
  - Render → Render Image，另存为 `projects/week01/donut_day1.png`
  - git add projects/week01/donut_day1.png
  - git commit -m "week01-day01: open donut lesson1 render — refs: https://github.com/thecrazymage/Blender-Donut-Tutorial"
  - git push --set-upstream origin week01-day01
- GitHub 网页操作：
  - 打开你的仓库 → Issues → New issue，标题写：`week01-day01 — Donut lesson1`，正文填入目标、参考教程 URL（粘上 thecrazymage 仓库链接）并创建 Issue

Day2 — Donut 基础建模（打开具体教程文件 / 本地操作）
- 打开：
  - https://github.com/thecrazymage/Blender-Donut-Tutorial
  - 在文件列表选择 lesson2.blend（或教程提供的第 2 步文件）并下载
- 本地：按教程在 Blender 中执行移动/缩放/挤出/环切，保存为 `projects/week01/donut_step2.blend`，渲染并保存 `projects/week01/donut_step2.png`
- Git 操作：
  - git add projects/week01/donut_step2.*
  - git commit -m "week01-day02: donut basic modeling step2 — refs: https://github.com/thecrazymage/Blender-Donut-Tutorial"
  - git push
- GitHub 页面：在 Issue（或新 Issue）中贴上本次 commit 的文件路径和简短问题/心得

Day3 — 材质与 Shader（跟练并保存中间状态）
- 打开：Donut 仓库（同上）并定位含材质说明的 lesson 文件或 README
- 本地：按教程在 Shader Editor 中添加 Principled BSDF，保存 `projects/week01/donut_step3.blend`，渲染导出 `donut_step3.png`
- Git：commit 并 push（参照 day2 的 commit 样式），并在 Issue 中更新进度

Day4 — 阅读 Mark 的文字课程并做 lesson01（打开具体文件）
- 打开：
  - https://github.com/Mark-McCormack/Blender-Course-Notes
  - 点击 Code → 进入 `lessons/` 目录： https://github.com/Mark-McCormack/Blender-Course-Notes/tree/main/lessons
  - 点击 `lessons/01.md`（或按顺序的第一课）并逐条执行文字步骤
- 本地：完成练习并保存为 `projects/week01/lesson01_from_mark.blend`，渲染截图
- Git：commit/push 并在你的 Issue 中引用具体文件 URL（例如 refs: https://github.com/Mark-McCormack/Blender-Course-Notes/blob/main/lessons/01.md）

Day5 — 对照 Donut 与 Mark 重做并写 notes（打开两处页面对照）
- 打开两个页面（分别在两个标签）：
  - https://github.com/thecrazymage/Blender-Donut-Tutorial
  - https://github.com/Mark-McCormack/Blender-Course-Notes/tree/main/lessons
- 本地：选择 Donut 中的一步，按 Mark 的文字说明重做并保存为 `projects/week01/donut_rework.blend`，导出 `donut_rework.png`
- 在 `notes/daily_log.md` 中追加当天记录，格式：日期 / 目标 / 参考 GitHub 文件 URL / 问题 / 解决方法
- Git：commit/push

Day6 — Tristan 的速查练习（打开并参照 rtmg.md）
- 打开：
  - https://github.com/TristanCacqueray/learn-blender/blob/main/rtmg.md
  - https://github.com/TristanCacqueray/learn-blender/blob/main/README.md
- 本地：按 rtmg 中的快捷键/技巧重做前几日的某个步骤，保存为 `projects/week01/tristan_quicksteps.blend` 并导出对比图
- Git：commit/push 并在 Issue 中写下学到的 3 个快捷键与用途

Day7 — 汇总并发布到 docs（在 GitHub Pages 准备展示）
- 在本地：
  - 选择本周最满意的 2 张渲染图复制到 `docs/`（或 `docs/week01/`）
  - 新建 `docs/week01_README.md`，写明每项练习引用的 GitHub 教程源（必须写完整 URL）
  - 示例引用格式：
    - Donut lesson1 — https://github.com/thecrazymage/Blender-Donut-Tutorial
    - Mark lesson01 — https://github.com/Mark-McCormack/Blender-Course-Notes/blob/main/lessons/01.md
    - Tristan rtmg — https://github.com/TristanCacqueray/learn-blender/blob/main/rtmg.md
- Git：
  - git checkout -b week01-portfolio
  - git add docs/ projects/week01/ notes/
  - git commit -m "week01: add portfolio & summary — refs: https://github.com/thecrazymage/Blender-Donut-Tutorial, https://github.com/Mark-McCormack/Blender-Course-Notes, https://github.com/TristanCacqueray/learn-blender"
  - git push origin week01-portfolio
- 在 GitHub 网页：
  - 打开你的仓库 → Settings → Pages
  - 在 Pages 的 Source 选择 Branch: `week01-portfolio`，Folder: `/docs` → Save（GitHub 会返回 Pages URL，记下用于展示）

提交/Issue/Commit 规范（务必遵守用于可追溯）
- Commit message 模板：
  - `weekXX-dayYY: <简短说明> — refs: <GitHub tutorial URL>`
- Issue 标题模板：
  - `weekXX-dayYY: <任务名> — refs: <tutorial URL>`
- notes/daily_log.md 每日追加一行（日期 / 目标 / 参考 / 问题 / 解决）

关于大文件（如果你的 .blend >100MB）
- 打开 GitHub 文档页：https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage
- 在本地使用 Git LFS：
  - git lfs install
  - git lfs track "*.blend"
  - git add .gitattributes
  - git add <your .blend>
  - git commit -m "add large .blend via LFS"
  - git push

后续说明
- 我已经按你授权（仅 B）在你的仓库中添加了本文件，内容遵循你要求“教程有且只有来自 GitHub”的规则，并在文本中列出每天必须打开的具体 GitHub 页面与文件路径（thecrazymage / Mark-McCormack / TristanCacqueray）。
- 如果你希望我继续（例如自动创建 Day1~Day7 Issues 或添加 Actions workflow），回复 A/C/D/E 中的选项并确认授权。

祝你第一周学习顺利！按本 checklist 做完后把你的仓库链接贴给我，我会审阅你的 commits 并给出改进建议。
