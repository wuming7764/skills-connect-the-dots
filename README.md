<header>

<!--
  <<< Author notes: Course header >>>
  Include a 1280x640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280x640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

[English](https://github.com/skills/connect-the-dots) | 中文

> 本课程翻译自 Github Skills，全部课程请点击 [这里查看](https://www.github-zh.com/getting-started)

# 在 GitHub 仓库中建立关联与线索

_学习如何在 GitHub 仓库中高效地查找、追踪和关联信息。_

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: 处理重复的 issue

_欢迎来到本课程 :tada:_

GitHub 提供了非常实用的功能，可以帮助我们在不同内容之间建立引用关系。
例如，当你在评论中引用另一个 issue 或 pull request 的编号时，这个编号会自动变成可点击的链接。
同时，GitHub 还会在被引用的 issue 或 pull request 中自动添加“反向引用”，形成一个双向链接。
这种机制能让你清晰地追踪不同内容之间的关联关系。

![a screenshot of an issue linking to a PR, and a PR with a cross-reference to the issue](https://user-images.githubusercontent.com/6351798/172456846-2daec570-08b0-4ffa-a7cb-41acc50b836e.png)

在团队协作开发中，常常会出现重复的 issue。 例如，上图中 issue `#8346` 实际上与之前的 `#8249` 问题重复。
通过 GitHub 的“交叉引用”功能，我们可以很轻松追踪这些重复项，并在合适的时候关闭重复的 issue。

### 创建引用

当你在 GitHub 中链接到另一个 issue 或 pull request 时，系统会自动生成引用。
同时你不需要粘贴完整的链接，只要在评论中输入 `#5`，GitHub 就会自动识别并生成指向编号为 5 的 issue 或 pull request 的链接。

如果想更精准地引用，可以在输入 `#` 后直接开始输入目标 issue 或 pull request 的标题，GitHub 会自动补全。
想进一步了解，可以参考文档：[自动链接引用与 URL](https://docs.github.com/en/articles/autolinked-references-and-urls)。

### :keyboard: 实操环节: 找到并关闭重复的 issue

1. 打开 issue #1 (Welcome)
2. 在评论区输入：`Duplicate of #2`，然后关闭 issue #1。
3. 等待大约 20 秒，再刷新此教程页面。[GitHub Actions](https://docs.github.com/en/actions) 会自动检测并更新课程进度，进入下一步。

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/connect-the-dots) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
