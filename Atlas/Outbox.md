up:: [[主页]]
tags:: #map/view 

# Outbox 📤
这里是一个跟踪各种 _输出_ 的地方。

下面是一个简单的数据视图示例，它正在查找任何带有标签`output`的笔记。

这已经足以让您入门。随着时间的推移，您可能还需要额外的自定义视图。

```dataview
TABLE WITHOUT ID
 file.link as Outputs,
 tags as Tags
 
FROM #output 

SORT file.name asc
```
