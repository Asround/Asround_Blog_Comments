# Asround_Blog_Comments

[Asround 博客](https://asround-blog.pages.dev/)的文章评论仓库，通过 [giscus](https://giscus.app/zh-CN) 展示 GitHub Discussions 中的留言。

- [查看评论与回复](https://github.com/Asround/Asround_Blog_Comments/discussions)：文章讨论位于“文章评论”分类。
- [博客源码](https://github.com/Asround/Asround_Blog)：评论组件、阅读工具栏和样式在博客源码中维护。
- 本仓库的 `giscus.json` 管理允许嵌入评论的站点地址和默认评论排序。域名或本地预览端口变化时需同步更新。

## 留言与通知

读者使用 GitHub 账号登录后发言，支持 Markdown、代码块和数学公式。行内公式示例：``$`E=mc^2`$``；行间公式使用独占一行的 `$$`。

留言及发言账号公开可见。可以在对应 Discussion 中订阅回复；是否发送邮件由个人 GitHub 通知设置控制。

评论默认按最新优先显示；`giscus.json` 中的 `defaultCommentOrder` 设为 `newest`。改为 `oldest` 可恢复最早优先，不会修改或删除已有留言。

## 维护

“文章评论”分类使用 Announcement 格式，由 giscus 为文章自动创建讨论，读者可以评论和回复。管理员可通过 Discussions 管理留言、锁定讨论或处理滥用内容。

评论数据保存在 GitHub Discussions 中，不是 Git 文件，因此克隆或拉取仓库不会下载评论数据。配置文件在 `main` 分支维护，本仓库无需构建或部署。

不要删除或随意更换既有讨论、分类与文章评论标识，以免已有留言失去关联。配置文件中仅保留公开信息，不存放访问令牌或其他密钥。
