up:: [[主页]]

tags:: #map #effort 

rank:: 5

# 我的邮件订阅 MOC

这个笔记是一个简单的例子，展示了如何将与某个项目相关的所有笔记整合到一个地方。以下是一个数据视图，可以查找 “Spaces” 中 `我的邮件订阅` 文件夹中的笔记。

``` dataview
TABLE WITHOUT ID
 file.link as "Newsletter",
 dates as "发布日期"

FROM "Spaces/我的邮件订阅"

SORT file.link desc

LIMIT 20
```
