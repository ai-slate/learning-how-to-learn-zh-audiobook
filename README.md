# 学会学习 · 中文有声读物

**把通勤、散步和休息的零碎时间，用来理解怎样更好地学习。**

学了又忘、迟迟不想开始、练了很多却仍不熟练——你可以从这里探索背后的原因，找到值得尝试的学习方法。41 节中文音频与配套正文，带你了解专注与发散思维、组块、拖延、记忆和考试准备；按自己的节奏听，也可以随时回到文字中复习。

**[开始在线收听 →](https://ai-slate.github.io/learning-how-to-learn-zh-audiobook/)** · [查看章节目录](#章节目录)

手机和电脑均可收听，支持倍速、连续播放、记住上次进度与章节下载。总时长约 **3 小时 2 分钟**，多数章节约 2–6 分钟，可以从最关心的主题开始。

## 你可以从这里获得什么

| 你关心的问题 | 可以探索的方法 | 推荐章节 |
| --- | --- | --- |
| 遇到难题，越想越卡住 | 理解专注与发散思维，给思考安排不同的节奏 | 01–03 |
| 看懂了，却没有真正掌握 | 认识组块、能力错觉与交错练习，重新检查练习方式 | 11–18 |
| 想开始学习，却一再拖延 | 把注意力放在过程、习惯与可开始的小步骤上 | 21–26 |
| 记住很难，遗忘很快 | 探索有意义的联结、长期记忆与记忆宫殿 | 27–30 |
| 希望更有条理地准备考试 | 回顾测试清单、先难后易与答案检查的方法 | 37–39 |

听完一节后，可以挑一个与你有关的方法，在下一次学习中尝试；遇到不熟悉的概念，就边听边看正文。这里适合学生、备考者，以及工作后仍在持续学习的人。具体收获取决于你的理解、练习和使用情境。

本项目基于 Barbara Oakley 与 Terrence Sejnowski 主讲的 **Learning How to Learn** 课程讲稿，按原讲稿标题编排为 **41 个章节**。

这是课程讲稿的中文翻译与有声改编，不代表课程方、原作者或平台的官方发行。制作使用了 AI 辅助翻译、语音合成及背景音乐生成，正文和发音仍可能存在需要校订之处。

- 仓库：[`ai-slate/learning-how-to-learn-zh-audiobook`](https://github.com/ai-slate/learning-how-to-learn-zh-audiobook)
- 在线收听：<https://ai-slate.github.io/learning-how-to-learn-zh-audiobook/>
- 原课程：[Learning How to Learn](https://www.coursera.org/learn/learning-how-to-learn)
- 内容来源与版权：[COPYRIGHT.md](COPYRIGHT.md)
- 播放器代码许可：[LICENSE](LICENSE)（MIT，仅适用于原创播放器代码与原创技术说明；不包含课程正文、译文或音频）

## 收听与阅读

进入网页后，选择章节并点击播放即可。页面同时展示该节中文正文，支持电脑、平板和手机。

| 功能 | 使用方式 |
| --- | --- |
| 章节选择 | 在目录中选择；手机上先展开目录。播放器中的章节标题也能带你回到目录。 |
| 播放 / 暂停 | 点击底部播放按钮。首次播放需要手动操作。 |
| 上一节 / 下一节 | 使用播放器两侧的章节切换按钮。 |
| 快退 / 快进 | 分别后退 15 秒、前进 30 秒；也可以拖动进度条。 |
| 倍速 | 点击倍速按钮，选择 0.9×、1×、1.1× 或 1.25×。 |
| 连续播放 | 打开“连播”，当前章节结束后尝试播放下一节。 |
| 续听 | 在同一浏览器中再次打开，恢复上次章节、播放位置、倍速和连播设置。 |
| 下载 | 正文上方的“下载本节音频”可保存当前章节 MP3。 |

键盘也可操作播放器：进度条获得焦点后，左右或上下方向键调整 5 秒，PageUp / PageDown 调整 30 秒，Home / End 跳到开始 / 结尾；倍速菜单支持方向键选择和 Escape 关闭。

手机浏览器可能限制自动播放、后台播放和锁屏后的连续切章。如果下一节没有自动开始，请回到页面点击播放。本站没有经过所有真机和浏览器组合的验证，不能保证每种后台播放行为。

## 本地使用

不需要安装 AudioStudio、Python、Node.js、数据库或模型。网页与音频均已生成。

1. 在仓库页面选择 **Code → Download ZIP**，下载并解压。
2. 打开 `docs/index.html`，确保同目录的 41 个 MP3 文件都在。
3. 如果浏览器限制本地文件访问或不能保存续听位置，可改用在线页面，或用已有的静态服务器托管 `docs/`。

已有 Python 3 时，可在仓库根目录运行简单的本地预览：

```bash
python3 -m http.server 8000 --directory docs
```

随后访问 `http://localhost:8000/`。这条命令用于预览；完整的音频跳转和续听体验需要托管服务器支持 HTTP Range 请求。正式在线收听使用 GitHub Pages。

网页没有自动缓存整本书的 Service Worker。在线访问时按当前章节请求音频；下载完整仓库后，本地文件可供离线收听。浏览器是否保存本地文件页面的阅读进度，取决于其对 `file://` 与本地存储的支持。

## 浏览器、字体与隐私

- 页面使用标准 HTML、CSS 和 JavaScript；建议使用当前版本的 Chrome、Edge、Firefox 或 Safari。手机端按窄屏与触摸操作设计。
- 不引入第三方字体、字体 CDN、外部脚本、图片 CDN 或统计 SDK。中文正文使用系统字体栈，如苹方、微软雅黑、冬青黑体，缺失时回退到浏览器系统字体。
- 正文在桌面端为 18px，窄屏为 17px，行高为 1.95；字体的具体呈现会随系统变化。
- 页面没有登录、评论、反馈表单、上传、评分或用户信息输入框。
- 续听数据只写入当前浏览器的 `localStorage`，包含章节、位置和播放设置。清理网站数据、使用无痕模式、更换设备或切换网站域名后，记录可能消失，不提供跨设备同步。
- 本项目没有收集续听记录的服务端。GitHub 作为托管平台的网络请求记录和隐私处理，适用其自己的政策。

## 仓库内容

```text
learning-how-to-learn-zh-audiobook/
├── README.md
├── COPYRIGHT.md
├── LICENSE
├── .gitignore
└── docs/
    ├── .nojekyll
    ├── index.html
    ├── chapter-001.mp3
    ├── …
    └── chapter-041.mp3
```

共 **47 个文件**，其中 `docs/` 是完整的网站发布目录。CSS、JavaScript 和中文正文均内嵌在 `index.html` 中，音频按章使用相对路径加载。

仓库仅包含收听所需的成品与必要说明，不包含原 PDF、英文抽取稿、翻译工作文件、朗读修订稿、候选声音、分段音频、WAV、中间混音、模型权重、数据库、凭证、日志、截图、测试报告或 ZIP 包。无需单独的 `book.json`，页面已经包含中文正文和章节元数据。

`.gitignore` 采用白名单，只允许本 README、版权说明、代码许可、网页和 `chapter-001.mp3` 至 `chapter-041.mp3`。它能降低误上传风险，但维护者仍需在每次提交前检查暂存文件；强制添加和修改白名单可以绕过这层保护。

## 在 GitHub Pages 发布

本项目使用 **`main` 分支的 `/docs` 目录** 发布。无需自行配置构建工具或 Actions 工作流，`.nojekyll` 用于直接发布静态文件。

1. 创建公开仓库 `learning-how-to-learn-zh-audiobook`，不勾选自动添加 README、`.gitignore` 或许可证；上传本仓库已准备的文件并保留目录结构。
2. 在 **Settings → Pages → Build and deployment** 中选择 **Deploy from a branch**。
3. 将分支设为 **main**，目录设为 **/docs**，保存。
4. 等待 GitHub Pages 部署完成，访问上方在线地址，并确认 HTTPS 可用。
5. 打开第一节、最后一节及任意中间章节，检查播放、拖动进度、倍速、连播与手机布局。

GitHub Pages 对应项目路径而非域名根路径。音频链接使用 `chapter-001.mp3` 这样的相对地址，不使用 `/chapter-001.mp3`。不要改变文件名大小写，也不要只上传 HTML。复制仓库到其他账号时，应同步更新 README 中的仓库、收听和版权联系链接。

部署参考：[配置发布源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)、[HTTPS](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)。

### 文件大小与带宽

41 节音频合计 **111,877,029 字节**（约 111.9 MB / 106.7 MiB），最大单节约 **5.0 MiB**。音频直接作为普通 Git 文件分发，**不使用 Git LFS**；GitHub Pages 不支持 Git LFS。

截至 2026-10-05，GitHub 对单个普通 Git 文件的硬限制为 100 MiB，Pages 发布站点的大小限制为 1 GB，流量软限制为每月 100 GB。按完整收听下载约 112 MB 粗略估算，这一软流量额度约对应 890 次完整音频传输；实际消耗受缓存、重复加载、拖动进度和访问量影响，并不等同于独立听众人数。

访问量增长后，可评估独立音频托管或更小的音频编码。不要把大体积、内嵌全书音频的离线 HTML 加入仓库，也不要反复提交音频大文件来累积无用历史。

官方说明：[普通 Git 文件大小](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github)、[Pages 限制](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)、[Git LFS 与 Pages](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage)。托管额度以 GitHub 最新规定为准。

## 章节目录

时长按成品音频取整；合计精确时长为 10,922.36 秒。以下链接可直接打开各节 MP3，网页中还可同步阅读正文。

| 序号 | 章节 | 时长 | 音频 |
| --- | --- | --- | --- |
| 01 | 专注模式与发散模式简介 | 04:22 | [MP3](docs/chapter-001.mp3) |
| 02 | 特伦斯·塞诺斯基与芭芭拉·奥克利 - 课程结构介绍 | 03:13 | [MP3](docs/chapter-002.mp3) |
| 03 | 使用专注模式与发散模式——或者，一点达利式的做法 | 03:36 | [MP3](docs/chapter-003.mp3) |
| 04 | 什么是学习？ | 05:35 | [MP3](docs/chapter-004.mp3) |
| 05 | 拖延症预览 | 02:30 | [MP3](docs/chapter-005.mp3) |
| 06 | 熟能生巧 | 05:37 | [MP3](docs/chapter-006.mp3) |
| 07 | 记忆简介 | 04:23 | [MP3](docs/chapter-007.mp3) |
| 08 | 睡眠在学习中的重要性 | 02:59 | [MP3](docs/chapter-008.mp3) |
| 09 | 模块1总结视频 | 04:08 | [MP3](docs/chapter-009.mp3) |
| 10 | 对接下来内容的期待！玛丽·安·内斯托尔给出特别提示 | 01:39 | [MP3](docs/chapter-010.mp3) |
| 11 | 组块简介 | 01:05 | [MP3](docs/chapter-011.mp3) |
| 12 | 什么是组块？ | 05:30 | [MP3](docs/chapter-012.mp3) |
| 13 | 如何形成组块 – 第一部分 | 04:48 | [MP3](docs/chapter-013.mp3) |
| 14 | 如何形成组块 – 第二部分 | 06:26 | [MP3](docs/chapter-014.mp3) |
| 15 | 能力错觉 | 07:29 | [MP3](docs/chapter-015.mp3) |
| 16 | 什么在激励你？ | 05:00 | [MP3](docs/chapter-016.mp3) |
| 17 | 组块图书馆的价值 | 05:17 | [MP3](docs/chapter-017.mp3) |
| 18 | 过度学习、紧张失常、定势效应与交错练习 | 08:29 | [MP3](docs/chapter-018.mp3) |
| 19 | 第二周总结 | 03:21 | [MP3](docs/chapter-019.mp3) |
| 20 | 拖延与记忆简介 | 01:11 | [MP3](docs/chapter-020.mp3) |
| 21 | 应对拖延症：它比你想象的更容易，也更有价值 | 06:02 | [MP3](docs/chapter-021.mp3) |
| 22 | 到处都是僵尸 | 03:24 | [MP3](docs/chapter-022.mp3) |
| 23 | 乘风破浪：过程与结果 | 04:00 | [MP3](docs/chapter-023.mp3) |
| 24 | 利用你的僵尸力量来帮助你 | 05:23 | [MP3](docs/chapter-024.mp3) |
| 25 | 在生活和学习的平衡中 | 05:34 | [MP3](docs/chapter-025.mp3) |
| 26 | 总结拖延症 | 01:56 | [MP3](docs/chapter-026.mp3) |
| 27 | 深入探索记忆 | 06:37 | [MP3](docs/chapter-027.mp3) |
| 28 | 什么是长期记忆？ | 05:01 | [MP3](docs/chapter-028.mp3) |
| 29 | 创建有意义的组块与记忆宫殿技术 | 06:23 | [MP3](docs/chapter-029.mp3) |
| 30 | 总结记忆 | 02:57 | [MP3](docs/chapter-030.mp3) |
| 31 | 如何成为更好的学习者 | 05:14 | [MP3](docs/chapter-031.mp3) |
| 32 | 文艺复兴式学习与释放你的潜能简介 | 01:38 | [MP3](docs/chapter-032.mp3) |
| 33 | 创造一个生动的视觉隐喻类比 | 03:34 | [MP3](docs/chapter-033.mp3) |
| 34 | 无需嫉妒天才 | 06:21 | [MP3](docs/chapter-034.mp3) |
| 35 | 改变你的思维，改变你的人生 | 05:45 | [MP3](docs/chapter-035.mp3) |
| 36 | 团队合作的价值 | 05:53 | [MP3](docs/chapter-036.mp3) |
| 37 | 一份测试清单 | 03:14 | [MP3](docs/chapter-037.mp3) |
| 38 | 先难后易 | 04:39 | [MP3](docs/chapter-038.mp3) |
| 39 | 考试最后的实用建议 | 05:38 | [MP3](docs/chapter-039.mp3) |
| 40 | 第四周总结 | 03:11 | [MP3](docs/chapter-040.mp3) |
| 41 | 特伦斯·塞诺斯基和芭芭拉·奥克利对课程的总结 | 03:03 | [MP3](docs/chapter-041.mp3) |

## 制作说明与验证范围

中文正文以提供的课程 PDF 讲稿为基础，按标题分节，经 AI 辅助翻译与朗读文本调整后生成音频。语音使用本地 **mlx-audio / Qwen3-TTS 1.7B CustomVoice / Serena**，采用听感对比中选定的清晰咬字方案；背景音乐使用本地 **ACE-Step** 生成，已混合进每节 MP3 中。听众无需分别加载人声和音乐，也无需在页面选择模型或音色。

同一节的语音片段已拼接为完整章节，音色和生成参数在制作时固定。网页倍速仅改变成品的播放速度，不会调用模型重新合成。成品音频已经包含配乐，网页没有单独的人声 / 音乐音量控制。

生成工具参考：AudioStudio、[mlx-audio](https://github.com/Blaizzy/mlx-audio)、[Qwen3-TTS 模型](https://huggingface.co/Qwen/Qwen3-TTS-12Hz-1.7B-CustomVoice)、[ACE-Step](https://github.com/ace-step/ACE-Step)。工具和模型的许可不等同于原讲稿、翻译与有声改编的内容许可；本仓库不分发模型文件。

本次制作检查覆盖了 41 节音频的完整解码、样本数、文件 SHA-256、响度和峰值，并验证中文正文的 294 段内容完整。播放器在本地浏览器验证了各节播放、倍速、连播、续听、下载及多种屏幕宽度。**尚未进行整书逐句人工校译和长时间人工听审**，这些技术检查不代表内容与听感已经由人工全面验收。

本说明记录的是发布准备时的验证。GitHub Pages 的公网播放需要首次部署成功后另行核实；完整测试记录与过程材料保留在制作环境，不纳入这个分发仓库。

## 维护与勘误

文字校订与音频更新是两件事：只改网页正文不会改变已经合成的朗读。涉及朗读错误时，需要同时更新对应 MP3 和 HTML 中该章的内容及 `sha256`。

保留同一本书的 `book_id` 和章节 `key`，可维持续听记录的归属；章节音频变化时必须更新 `sha256`，播放器会舍弃该章旧音频的位置记录，避免错误续听。新增、删除或重排章节时，还需同步目录、`expected_chapters`、`.gitignore` 的章节白名单和本 README。

更新前检查实际暂存文件、章节数、相对路径和音频哈希；更新后确认 GitHub Pages 的部署完成，并在手机和桌面端检查页面。不要将工作文件放进 `docs/`，因为该目录下的文件可能直接被公开访问。

内容勘误可通过仓库 Issue 提交，注明章节标题和音频时间点。网页本身不设置反馈入口。

## 内容来源、版权与联系

原创播放器的 HTML 结构、CSS、JavaScript 与原创技术说明采用 [MIT 许可](LICENSE)。内嵌在同一 HTML 中的课程正文、中文译文，以及全部音频不在这项代码许可的范围内；复制播放器代码时须保留版权和许可声明。不同类型的材料分别说明许可范围，参考 [GitHub 的混合内容许可说明](https://choosealicense.com/non-software/)。

原课程由 Barbara Oakley 与 Terrence Sejnowski 主讲。原讲稿、相关课程内容及其既有权利归原作者或相应权利人所有。本项目是独立整理的中文翻译与有声改编，其公开分发授权尚未确认，也不对原始内容、译文或音频追加统一的开放内容许可。

**我们尊重原作者及相关权利人的合法权益。若您是本项目所涉内容的权利人或其合法代理人，并认为本项目的文字、译文、音频或其他内容涉及您的权益，请通过[本仓库 Issue](https://github.com/ai-slate/learning-how-to-learn-zh-audiobook/issues) 联系维护者，注明相关内容或章节、您的身份及权利依据。收到有效说明后，我们将及时核实，并根据核实结果调整、下架或删除相关内容。**

请勿在公开 Issue 中上传身份证件、合同、住址或其他敏感资料；如需进一步核实，维护者将协商合适的沟通方式。教学与学习分享的目的及上述联系声明，不能替代权利人的授权。进一步说明见 [COPYRIGHT.md](COPYRIGHT.md)。
