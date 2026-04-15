<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: 查找历史提交记录

_你已成功关闭那个重复的问题 :wave:_

git 这类版本控制工具的一大优势，是可以回溯文件的修改历史记录。使用 `git blame` 命令，我们不仅能看到是谁修改了代码，还能了解为什么要进行这次修改。
比如：

- 这个提交对应的是哪个 pull request？
- 谁审核并通过了它？
- 在合并前是否运行过测试？

这些信息能帮助我们更全面地理解项目的演变过程，而不仅仅是看到“谁改了什么”。

### 什么是 `git blame`?

`git blame` 是一个 Git 命令，用于逐行查看文件的修改历史。它会显示文件中每一行代码最后一次是由谁、在什么时候修改的。
它能让你找到修改记录的作者、时间，甚至能帮助你推断修改背后的原因。

虽然 “blame” 翻译过来有 “责备” 的意思，但它的真正用途并不是“追责”，而是帮助我们**理解决策背景**、理清代码的演变脉络。

### 什么是 SHA（安全哈希算法）?

SHA 是 Git 用来标识对象（如提交、文件、树等）的唯一标识符。 在这里，我们主要关注的是 **commit 的 SHA 值**。
每个提交都会有一个 40 位的十六进制字符串（例如 `a1b2c3d4e5f6...`），用来唯一表示该次提交。

在 GitHub 上，你可以点击任意一个 commit 查看：

- 该提交中修改的内容。
- 提交者是谁.
- 它是否属于某个 pull request。

### :keyboard: 实操环节: 查找历史提交记录

现在需要你找到引发 issue #2 问题的 commit 记录。

1. 进入你仓库的 **Code**（代码）页面。
2. 打开 `docs` 目录。
3. 点击 `_sidebar.md` 文件以查看内容。
4. 在文件上方，点击 **Blame** 按钮，查看该文件中每行的最后修改记录。
5. 找到提交信息为 `add sidebar to documentation` 的那一条，点击它进入 commit 详情页。
6. 复制该 commit 的 SHA 值的前 **7 个字符**（即 `commit` 后方那串 40 位十六进制字符串的前 7 位）。
7. 打开 issue **#2**，在评论区中粘贴刚复制的 7 位 SHA 值，并点击 **Comment**。
8. 等待大约 20 秒，然后刷新此页面（即本教程页面）。[GitHub Actions](https://docs.github.com/en/actions) 会自动检测进度并进入下一步。