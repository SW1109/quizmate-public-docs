---
layout: page
title: 操作手册
permalink: /guide/
---

适用插件 **0.9.0**，更新于 **2026 年 11 月 13 日**。本手册说明卡密兑换、练习、网课、设置与故障处理。第一次使用可先看[Edge 安装到首次使用](EDGE_START.md)。

**版本提醒：** 2026 年 11 月 13 日核对时，Edge 商店仍提供 0.8.1。本文截图为 0.9.0；商店更新前，旧版“开始答题”对应新版“开始练习”，“仅查看答案”对应“只看答案”，“开始前设置”对应“首次使用”。不要为更新而卸载原插件，以免丢失本机授权和配置。

## 1. 在 Edge 安装插件

1. 在 Microsoft Edge 电脑版打开[QuizMate 商店页面](https://microsoftedge.microsoft.com/addons/detail/quizmate/nmkgnejillemkmplbkcklhdcfkgefoce?hl=zh-CN)。
2. 核对名称 **QuizMate · 智答伴侣**，发布者 **Nexly 光年数智工作室**。
3. 点击 **获取**，阅读权限提示后确认 **添加扩展**，等待浏览器提示安装完成。
4. 打开工具栏的 **扩展**菜单，找到 QuizMate，选择 **在工具栏中显示**。部分 Edge 版本使用眼睛或固定图标。
5. 打开一页允许使用辅助工具的学习练习，点击工具栏里的 QuizMate 图标，打开右侧学习侧栏。

<figure class="guide-figure"><a href="/quizmate-public-docs/assets/guide/v0.9.0/edge-store.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/edge-store.png" alt="微软商店中的 QuizMate 名称、图标和发布者" width="752" height="110"></a><figcaption>实际商店条目，核对名称和发布者即可。此图仅展示识别信息。</figcaption></figure>

商店安装不需要开启开发者模式。若网页提示“与浏览器不兼容”，请确认链接是在 **Microsoft Edge** 中打开。找不到图标时，在地址栏打开 `edge://extensions`，确认插件已启用，且使用的是安装时的浏览器个人资料。

## 2. 认识三个使用入口

| 入口 | 用来做什么 |
| --- | --- |
| 学习侧栏 | 操作当前网页：首次设置、练习、网课和最近进度。 |
| 工作台 | 管理卡密与额度、答题服务、练习和网课设置，查看完整题目与记录。 |
| 网页悬浮按钮 | 在已授权网页上查看状态，开始、暂停、停止，或打开侧栏。 |

**侧栏跟随当前正在看的网页。** 操作前核对顶部的网页名称和网站地址。任务开始后绑定原网页，切换标签不会把运行中的任务改到新网页；出现 **返回任务网页** 时，点击回到原任务。

<figure class="guide-figure wide"><a href="/quizmate-public-docs/assets/guide/v0.9.0/workspace.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/workspace.png" alt="0.9.0 工作台的开始使用、我的网课、题目与答案和运行记录入口" width="1280" height="900" loading="lazy"></a><figcaption>0.9.0 工作台。截图中的卡密、题目和用量均为本地演示数据；下方插件截图同样如此。</figcaption></figure>

## 3. 兑换卡密并完成首次设置

在侧栏选择 **练习**，按“首次使用”中当前展开的一步操作：

1. 在 **收到的卡密**中粘贴完整的 QM 开头卡密，点击 **兑换卡密**，也可按 Enter。浏览器申请访问授权网站时，核对地址后允许。
2. 兑换成功会自动更新权益。仅有官方服务可用时会自动选好；时长卡开放 API 和本地模式，需要选一种并完成对应配置。
3. 阅读数据说明，勾选同意后点击 **确认并启用 AI 功能**。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/redeem.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/redeem.png" alt="首次使用中的卡密输入框和兑换按钮" width="400" height="920" loading="lazy"></a><figcaption>粘贴收到的卡密即可。默认授权地址已配置，无需另外填写。</figcaption></figure>

兑换后不用再手动核验或点击“保存设置”。如果原来已有可用的使用方式，插件会保留，不会自动改变计费方式。

官方服务卡用于 **官方服务（题库＋AI）**，不需要填写 API Key 或安装本地桥。时长卡用于 **API 模式／本地模式**，需要自己的模型接口或 CLI。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/consent.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/consent.png" alt="首次求解前的数据说明、同意复选框和确认按钮" width="400" height="920" loading="lazy"></a><figcaption>确认数据说明后才可调用 AI。网站读取权限仍由浏览器另行询问。</figcaption></figure>

## 4. 第一次练习

1. 登录学习网站，进入实际显示题干和选项的页面，等待内容加载完成。
2. 打开学习侧栏，核对 **当前网页**，完成首次设置。
3. 点击 **开始练习**。首次访问时按钮显示 **授权此网站并开始**，允许浏览器访问后会继续读取和处理。
4. 在侧栏查看进度，完成后核对网页上的结果。**最终提交由你操作。**

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/ready.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/ready.png" alt="服务准备完成后，侧栏显示剩余次数和开始练习按钮" width="400" height="920" loading="lazy"></a><figcaption>准备完成后的主操作。图中 70 次为演示套餐，实际权益以你的卡密为准。</figcaption></figure>

想先核对题目，可点 **查看当前题目**；已经读过时显示 **重新读取题目**。只读题不调用模型、不消耗额度。若识别到上一题或缺少选项，先重新读取，不要继续求解。

| 操作 | 结果 |
| --- | --- |
| 开始练习 | 读取并求解，满足填写条件后写入当前网页。 |
| 只看答案 | 求解并显示答案，不自动填写；同样可能消耗套餐次数。 |
| 填入答案 | 把当前预览答案填入原题，填写前仍会核对页面是否变化。 |
| 查看题目与答案详情 | 在工作台查看完整题面、答案和解释。 |

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/answer.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/answer.png" alt="仅预览时显示的本题答案与填入答案按钮" width="400" height="920" loading="lazy"></a><figcaption>本地示例题的答案预览。先核对答案，再决定是否填写。</figcaption></figure>

插件按当前选项内容核对答案，不能把其他题目或其他选项顺序的答案字母直接套用。置信度达到阈值也不代表答案一定正确。

## 5. 连续练习与暂停

进入 **设置 → 练习设置**，可调整每批题数，范围 **1～200 题**，默认 **100 题**。设置会在下次任务开始时生效。

| 操作或状态 | 怎么处理 |
| --- | --- |
| 暂停 | 暂时停止后续处理；确认页面未变化后可继续。 |
| 继续 | 接着处理原任务，不会改绑到当前新开的网页。 |
| 停止 | 结束本批任务，保留网页上已经填写的内容。 |
| 正在读取 | 读取期间可停止，不能暂停。 |
| 任务在另一个网页 | 点击“返回任务网页”，再查看进度或停止。 |

**答题期间保留原网页标签，不要关闭、刷新或退出浏览器。** 收起侧栏不会停止任务。开启“切换标签后继续作答”也不能让已关闭的页面继续运行。

## 6. 编程题与作业

编程题先等待编辑器加载，再读取并检查题目、语言及当前代码。可在练习设置中开启填写后执行页面样例；失败时最多额外修正 **2 次**，修正会发送当前代码和可见执行日志，可能产生额外用量。

代码完成后，由你检查、提交并按页面提示换题。编辑器不可写、按钮禁用或有多个不明确入口时，应先在网页处理，插件不会猜测操作目标。

作业页会根据实际页面显示 **生成参考草稿**、**仅预览草稿**或 **录入文章**。只有说明、没有完整正文题目时不会求解。参考内容需自行核对字数、事实和表达，再按平台要求保存和提交。

## 7. 网课学习

支持超星学习通、智慧树、中国大学 MOOC 和国家开放大学实验学院部分页面。不同播放器和页面的兼容情况可能不同。

1. 在课程网站完成登录，打开实际视频或支持的 HTML 文档，展开章节目录。
2. 在该网页打开侧栏，选择 **网课**。
3. 可先点 **识别课程**检查目录，也可直接点 **开始学习**，由插件先识别再启动。
4. 按需要暂停、继续、停止，或展开 **章节目录**选择已解锁章节。
5. 需要完整目录时点 **课程详情**。随堂练习有单独的查看答案和填写入口。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/sidebar-course.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/sidebar-course.png" alt="网课侧栏的学习操作、当前章节和章节目录" width="320" height="800" loading="lazy"></a><figcaption>本地模拟课程。课程进度显示不等于平台已经确认完成。</figcaption></figure>

课程识别和正常播放不需要卡密；随堂解题需要有效的答题服务和数据使用同意。**网课设置**里可调整播放速度、自动下一章和等待时间。默认 1 倍速，换章等待 3 秒，无进度 120 秒暂停；可选倍速不代表网页播放器一定支持。

遇到登录、验证码、锁定章节、PDF 或不支持的播放器时，在原网站处理。视频开始或继续时会静音，播放中可手动取消静音。

## 8. 工作台 设置与运行记录

侧栏点 **设置**打开完整工作台；点 **全部记录**查看练习和课程记录。

| 设置分类 | 常用操作 |
| --- | --- |
| 卡密与额度 | 兑换、刷新剩余时长、查看次数与余额、退出授权。 |
| 答题服务 | 选择当前有权限的模式，配置 API 或检查本地桥。 |
| 练习设置 | 每批题数、后台运行、代码样例与填写节奏。 |
| 网课设置 | 播放速度、换章和无进度处理。 |
| 悬浮按钮 | 是否自动显示、透明度、重置位置。 |
| 隐私与帮助 | 使用帮助、反馈和数据使用同意。 |

侧栏底部的 **最近进度**可展开或收起，支持按来源筛选和搜索。查看旧记录时，新日志不会强制把你拉回顶部；点击“回到最新”可继续跟踪。

<figure class="guide-figure wide"><a href="/quizmate-public-docs/assets/guide/v0.9.0/floating.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/floating.png" alt="学习网页上展开的 QuizMate 悬浮按钮" width="1280" height="900" loading="lazy"></a><figcaption>悬浮窗可固定、拖动和收起。打开侧栏可继续处理设置与错误。</figcaption></figure>

外观设置和主题会同步到工作台、侧栏与悬浮窗。任务设置需要保存，并在下次任务生效。清除本地记录不会删除服务器调用账本。

## 9. 中断或报错后的恢复

1. 先看中文提示和最近记录，确认是页面、连接还是卡密问题。
2. 网页已刷新或误关时，重新打开原练习，核对已经填写的内容，回到当前题目。
3. 点击 **重新读取网页**或 **查看当前题目**。此操作不调用模型。
4. 连接或额度异常时点 **检查连接与卡密**。确认状态后，再由你决定是否重新开始。

| 提示 | 下一步 |
| --- | --- |
| 找不到标签或 “No tab with id” | 原网页已关闭。重新打开题目页，在该页打开侧栏。 |
| 文档已变化或 “No document with id” | 题目区域刷新了。等待加载完成，核对后重新读取。 |
| 未读取到完整题目 | 打开具体题目，检查选项或编辑器是否已加载。 |
| 服务配置暂时无法读取 | 点击“重新检查服务”；卡密输入会保留。 |
| API 密钥已锁定 | 在答题服务设置里解锁，或重新填写密钥。 |
| 额度不足或待核对预占 | 查看卡密明细，等待结算或联系发卡方，避免连续重复请求。 |

停止或关页不能撤回已经发送给模型的请求。看到错误后不要连续点开始；先核对已填写内容、日志和用量。

## 10. 两类卡密与常见问题

| 卡密 | 可以使用 |
| --- | --- |
| 官方服务卡 | 官方题库与 AI。按套餐约定的次数、金额和期限使用；题库命中也扣一次套餐次数。 |
| 刷题时长卡 | 自配 API 和本地 CLI。首次激活后连续计时，离线也计时；模型费用由相应服务商收取。 |

两类卡可同时兑换，权益各自独立。没有权限的模式不会出现在选项中。同类新卡替换本机所选卡，不自动叠加期限；重复兑换同一张卡不会重置到期时间。

<figure class="guide-figure wide"><a href="/quizmate-public-docs/assets/guide/v0.9.0/license.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/license.png" alt="卡密与额度页的兑换入口和两类权益" width="1280" height="900" loading="lazy"></a><figcaption>未开通的卡种只显示状态。官方次数与金额以在线查询结果为准。</figcaption></figure>

**只看答案会扣次数吗？** 会发起求解，可能消耗套餐。单纯查看题目、识别课程和查询额度不会调用模型。

**官方卡能用自配 API 吗？** 不能。需要另有有效的时长卡；反过来，时长卡也不包含官方题库和模型额度。

**换电脑或重装后不能使用？** 卡密绑定安装实例。先联系发卡方核对绑定，不要反复卸载、兑换或更换浏览器个人资料。

## 11. 自配 API 与本地模式

仅在持有有效时长卡并准备使用自己的模型服务时配置。使用官方服务卡可跳过本节。

**API 模式**

1. 进入 **设置 → 答题服务**，选择 **API 模式**。
2. 选择服务商预设或填写兼容地址、API Key 和模型名称。
3. 点击 **保存设置**，按浏览器提示允许访问该接口域名。
4. 可点击 **测试连接**发送固定测试题；不读取当前网页，但服务商可能收费。

地址支持兼容 OpenAI 的 Chat Completions 或 Responses 接口；公网地址须使用 HTTPS。密钥默认仅保存在本次浏览器会话。启用口令加密保存后，重启浏览器需解锁，忘记口令需重新填写 Key。

**本地模式**

需要本机已安装 Node.js 22+、支持的 CLI 和本地桥，并在 CLI 完成登录。进入 **答题服务 → 本地模式 → 设置／修复本地桥**，按当前浏览器与扩展 ID 生成的命令安装，然后重新检测。

本地模式复用 CLI 的账号与配置，CLI 仍可能请求远程模型；插件不包含其订阅或模型额度。

<figure class="guide-figure wide"><a href="/quizmate-public-docs/assets/guide/v0.9.0/connection.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/connection.png" alt="答题服务设置，只展示当前卡密允许的模式" width="1280" height="900" loading="lazy"></a><figcaption>示例只兑换了官方卡，因此只有官方服务可选。API 和本地模式需有效时长卡。</figcaption></figure>

## 12. 更新与反馈

在 `edge://extensions` 核对插件版本，保留原安装和浏览器个人资料。商店版由浏览器检查更新；更新后，在下一次任务开始前刷新已打开的题目网页。运行中不要更新插件或刷新题目页。

卡密、绑定、期限、扣费和订单问题优先联系发卡方。反馈界面或兼容问题时，提供插件版本、浏览器版本、页面类型、复现步骤与脱敏截图。不要公开卡密、API Key、密码、Cookie 或私有题目。

[公开问题反馈](https://github.com/SW1109/quizmate-public-docs/issues) · [隐私政策](https://sw1109.github.io/quizmate-public-docs/privacy/) · [从 Edge 安装到首次使用](EDGE_START.md)
