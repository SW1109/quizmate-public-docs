---
layout: page
title: Edge 安装到使用
permalink: /edge-start/
---

适用于 Windows / macOS 的 Microsoft Edge 电脑版。更新于 **2026 年 11 月 13 日**，插件截图为 **0.9.0**。

本文按官方服务卡的使用流程说明。准备一张有效卡密和一个已登录的练习网页，即可从下面开始。自配 API 或本地 CLI 用户完成安装后，按[详细手册](GUIDE.md)配置自己的服务。

**商店版本：** 本次核对时仍为 0.8.1。旧版“开始答题”对应新版“开始练习”，“仅查看答案”对应“只看答案”，“开始前设置”对应“首次使用”；操作顺序相同，以安装后的实际界面为准。

## 1. 打开商店并安装

在 **Microsoft Edge** 中打开[QuizMate 商店页面](https://microsoftedge.microsoft.com/addons/detail/quizmate/nmkgnejillemkmplbkcklhdcfkgefoce?hl=zh-CN)。核对名称 **QuizMate · 智答伴侣**和发布者 **Nexly 光年数智工作室**，点击 **获取 → 添加扩展**。

<figure class="guide-figure"><a href="/quizmate-public-docs/assets/guide/v0.9.0/edge-store.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/edge-store.png" alt="在商店核对 QuizMate 的名称、图标与发布者" width="752" height="110"></a><figcaption>实际商店条目的识别信息。若提示浏览器不兼容，请用 Edge 打开链接。</figcaption></figure>

安装完成后，打开工具栏的 **扩展**菜单，将 QuizMate 设为 **在工具栏中显示**。部分版本显示为眼睛或固定图标。商店安装不需要开发者模式。

**完成标志：** 点击工具栏的 QuizMate 图标，浏览器右侧出现学习侧栏。

## 2. 打开题目网页

先登录自己的学习网站，进入显示完整题干和选项的练习页，等内容加载完成，再打开 QuizMate。

核对侧栏顶部的 **当前网页**。如果显示“请切换到课程或练习网页”，回到题目标签即可，侧栏会自动跟随。不要停留在扩展商店、浏览器设置页或插件工作台里读题。

## 3. 兑换卡密

在侧栏选择 **练习**，找到 **首次使用**，将收到的完整 QM 开头卡密粘贴到输入框，点击 **兑换卡密**。浏览器申请访问授权网站时，核对后允许。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/redeem.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/redeem.png" alt="侧栏首次使用中的卡密输入框与兑换按钮" width="400" height="920" loading="lazy"></a><figcaption>0.9.0 真实界面，本地演示环境。默认授权地址已配置。</figcaption></figure>

官方卡兑换后会自动更新权益，首次只有官方服务可用时自动选好。无需填写 API Key、安装 Node.js 或本地桥，也不用再手动核验。已有有效服务选择时会保留原设置。

## 4. 确认数据说明

阅读当前展开的数据说明，勾选同意，再点击 **确认并启用 AI 功能**。这一步说明求解时哪些练习数据会发送给所选服务商。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/consent.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/consent.png" alt="数据说明、同意复选框与确认按钮" width="400" height="920" loading="lazy"></a><figcaption>确认后显示当前答题服务。网站访问权限仍可能由浏览器另行询问。</figcaption></figure>

**完成标志：** 侧栏显示当前服务和 **开始练习**按钮。演示图中的套餐与剩余次数不代表实际购买权益。

## 5. 开始第一道练习

点击 **开始练习**；首次访问网站时，按钮会显示 **授权此网站并开始**。允许浏览器访问后，插件会读取当前题目，获取答案并按填写条件处理。

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/ready.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/ready.png" alt="已准备好的侧栏，包含开始练习和只看答案入口" width="400" height="920" loading="lazy"></a><figcaption>主按钮开始练习；“查看当前题目”只读题，“只看答案”会求解但不自动填写。</figcaption></figure>

想先检查题目，点 **查看当前题目**，此操作不调用模型。想先看答案，点 **只看答案**，确认后可再点 **填入答案**。官方题库命中和模型求解都可能消耗套餐次数，别反复点击开始。

## 6. 核对结果并结束

<figure class="guide-figure sidebar"><a href="/quizmate-public-docs/assets/guide/v0.9.0/answer.png" target="_blank" rel="noopener noreferrer"><img src="/quizmate-public-docs/assets/guide/v0.9.0/answer.png" alt="答案预览与填入答案按钮" width="400" height="920" loading="lazy"></a><figcaption>本地演示题的答案预览。答案与实际网页上的选择项需要自行核对。</figcaption></figure>

在网页核对填写结果，**最终提交由你操作**。临时离开点 **暂停**，结束本批点 **停止**。设置里可调整每批题数；“开始练习”可能继续处理下一题，不一定只处理一题。

**任务进行中不要关闭、刷新题目标签或退出浏览器。** 收起侧栏不等于停止任务。误关或刷新后，先核对已填写内容与用量，再重新读取当前题目并手动开始。

遇到问题先看中文提示：页面问题点 **重新读取网页**，连接或卡密问题点 **检查连接与卡密**。重新读取不会调用模型。

需要网课、编程题、两类卡密或 API 配置说明，请继续看[完整操作手册](GUIDE.md)。
