# Conditional DETR

原始项目链接: https://github.com/Atten4Vis/ConditionalDETR

Conditional DETR与DETR的主要不同:

1. matcher中的Loss计算部分与Deformable DETR是相同的，与DETR有些修改
2. SetCriterion中计算label loss使用了focal loss，与Deformable DETR是相同的，与DETR有些修改

其实很多小地方都是与Deformable DETR相同的

重点的几个不同的文件:
1. conditional detr
2. transformer
3. attention (这个文件是多出来的，因为conditional detr需要修改一些attention的约束限制)