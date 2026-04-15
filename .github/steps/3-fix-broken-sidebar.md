<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 3: 修复损坏的侧边栏

_很棒！你已经成功找到了那次错误的提交 :heart:_

通过上一步我们确认，侧边栏确实是在那次提交中被添加的。接下来，我们来看看能否进一步了解这次更改背后的背景信息——是否有相关讨论、评论或规划记录。

通过前面的学习我们知道，issue 和 pull request 中的讨论可以引用其他工作，但这些“交叉引用”只是 GitHub 协作的一部分。

- 提交者是谁；
- 这次提交还包含了哪些改动；
- 提交的时间；
- 该提交属于哪个 pull request。

Pull request 是理解项目历史的重要入口。 它不仅告诉你“提交是什么时候发生的”，更能揭示“**为什么**会发生这次提交”。
在查看历史记录时，我们关注的并不是“谁改错了”，而是希望从中看清全局：
- 决策是怎么形成的？
- 有哪些人参与了？
- 每次提交的构建和测试结果如何？
- 谁提出了修改建议，又是谁最终批准的？

### 查找 commit 对应的 pull request

在 GitHub 上查看某个 commit 时，可以看到非常详细的信息。除了提交信息，GitHub 还会自动显示该 commit 所属的 pull request 链接。
接下来我们将利用这个功能。

![screenshot of a view of a commit on GitHub, highlighting the link to the pull request](https://user-images.githubusercontent.com/16547949/67341250-3edbb480-f4fd-11e9-805a-6bce5a8ba2d1.png)

### :keyboard: 实操环节: 修复损坏的侧边栏

1. 在 main 分支中打开并编辑 [`docs/_sidebar.md`](/docs/_sidebar.md) 文件。
2. 找到第 4 行，将错误的链接地址 `(doc-references__.md)` 改为正确的 `(doc-references.md)`。
3. 在提交更改时，选择或新建一个分支 **`fix-sidebar`**。
4. 创建一个新的 pull request，确保 **base:** 为 `main`，**compare:** 为 `fix-sidebar`。
5. 在右侧 **Assignees** 区域中，将该 pull request 分配给自己。
6. 在 PR 评论中添加 `Closes #2`，以自动关联并关闭 issue #2。
7. 点击 **Create pull request** 创建 PR，并等待约 20 秒。
8. 合并该 pull request。
9. 删除分支 `fix-sidebar`。
10. 再等待大约 20 秒，然后刷新本教程页面。[GitHub Actions](https://docs.github.com/en/actions) 会自动检测进度并进入下一步。