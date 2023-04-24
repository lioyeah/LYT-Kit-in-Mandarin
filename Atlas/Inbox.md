up:: [[主页]]
tags:: #map/view 

# The Inbox

这不止是收件箱，还是一个散热垫🧊。

想法在刚产生的时候显得很热烈🌶，但过几天之后就会冷却下来 ❄️。

当较为冷静的想法占上风时，你就可以按优先度为它们排序。不错吧？

通过本视图查看 **+Encounters** 文件夹中最新的 20 篇笔记。在处理它们时，建立联系、添加详细信息、将其移动到最合适的文件夹中，并删除冗余的其他内容 ✨。

> [!HINT]+ 此数据视图🔬仅在免费下载版本中呈现。
> 如果你正在 Obsidian Publish 上查看此注释，则无法看到下方的生成内容，请 [下载工具包](https://www.linkingyourthinking.com/download-lyt-kit)。在我的库中，它看起来像这样
> ![[lyt-kit-example-cooling-pad-.jpg]] 
> 如果已经可以看到下面的列表，则 LYT 工具包已经就绪。

``` dataview
TABLE WITHOUT ID
 file.link as "Encounters and new notes",
 (date(today) - file.cday).day as "Days alive"

FROM "+ Encounters" and -#on/readme 

SORT file.cday asc

LIMIT 20
```


---

如果你想了解更多内容，可以前往: [🐦](https://www.twitter.com) or [📚](https://readwise.io/lyt/)          