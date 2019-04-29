## 优达学城DAND（进阶）P3-Tableau数据可视化
**初始版本**[链接](https://public.tableau.com/profile/evan5913#!/vizhome/mobike_shanghai_15559070799380/1 )   
**最终版本**[链接](https://public.tableau.com/profile/evan5913#!/vizhome/mobike_sh_final/sheet0?publish=yes)

## 优达DAND（进阶）P4-创建Tableau故事
数据集来源于摩拜单车上海地区2016年8月的骑行数据，样本共计102361条记录。

### 总结
- 8月骑行人数提升约三倍，人均骑行时长基本在15-20min之间；  
- 单车骑行主要在黄浦江西岸的上海市区，西区的骑行位置密度与东岸的浦东新区形成强烈对比；  
- 在工作日7-8点，17-19点有骑行数量激增，与工作早晚高峰相合，说明很多人以共享单车为通勤工具；
- 从逐日变化观察高峰时段骑行人次，总体骑行人数稳定增长，但存在个别高峰段（18h）人数相比前后时段陡降的现象。

### 设计
故事思路
- 故事共包含四个仪表盘，分别介绍了，总体的骑行人数和人均时间的变化，骑行地点分布，工作日/周末对比，以及基于逐日/小时二维的骑行人数变化。

图表类型  
- 骑行人次展示8月逐日的骑行人次，且使用颜色区分工作日/周末，因此选择柱状图，人均骑行时间若采用折线图会发生间断，因此使用圆点图；
- 为了展示骑行的位置分布，采用地图展示骑行起始位置分布；
- 为了比较工作日/周末的骑行人数/人均骑行时间的对比，采用小图组；
- 为了展示逐日/逐小时骑行人次的数量对比，采用热力图，采用大小方块表示骑行人次；

图表布局
- 故事中仪表盘4的热力图纵轴为日期，因此选择在纵轴左侧位置放置逐日的骑行人数变化；
- 故事中仪表盘4的热力图横轴为时间，因此选择在横轴上侧位置放置逐小时的骑行人数变化；

图表的图例
- 故事中图例采用较为统一的表示，所有柱状图中蓝色表示工作日，橙色表示周末，热力图中的方块大小表示骑行人次等。


### 反馈
<<<<<<< HEAD
**第一次提交**：  
- 他人反馈：  
 1. 周末/非周末骑行数量并非1比3；  
 2. 骑行人数中工作日/周末没有进行对比；  
- 修改：
 1. 修改了周末/非周末骑行人数的计算；
 2. 增加工作日/周末进行颜色标注。

**第二次提交**：  

1. 审阅意见： 既然你呈现的最终结果为一个故事，其他部分已经包含在故事中，那么可以将其隐藏，使得工作簿更加简洁。隐藏表可以使用下图的Hide all sheets实现：需要注意，如果只保留故事部分，你需要先在仪表板选项卡中隐藏工作表，再在故事选项卡中隐藏仪表板。

 - 修改：已经隐藏除故事外的其他工作簿和仪表盘。

2. 审阅意见：你的仪表板以及故事的尺寸较小，导致可视化内容比较拥挤，请在故事和各仪表板（二者均需要选择）的Size中选择Automatic以解决此问题（对于故事及所有故事点中的仪表板，都应当选择此选项）：选择“Automatic”还有一个重要理由，即每个人所使用的设备分辨率不尽相同，如果使用固定尺寸，会导致可视化在某些设备上无法合理展示。因此请对此部分进行适当调整。

 - 修改：将所有仪表盘和故事的视图修改为“自动”

3. 审阅意见：请注意，在故事中，你需要用文字说明从故事中得出的发现和结论（在故事的标题处或使用单独的文本框），而不仅仅是展示标题或者对可视化进行非常简单的概括。观众需要从你的文字叙述中，深入理解每幅图表并对你得出的结论有清晰认知，以了解你的分析目的和成果。目前你制作的热力图中，并无具体的文字说明。请参考此链接完善了解为了制作一个优秀的故事应当遵循的规范，并在下次提交时补充文字说明；

 - 修改：在故事标题4中详细描述了发现和结论，并对其他故事进行完善。
 
4. 审阅意见：故事点1，折线已经无法看清，大部分被条形图遮盖。请调整透明度或使用小图组等方式使折线能清晰显示；

 - 修改：使用小图组展现条形图和折线图，但折线图并不连续（因为工作日/周末颜色的差异），而修改为了圆点图
 
 
5. 审阅意见： 你的项目报告的“设计”部分不符合要求。你需要在设计中说明所做故事包含的：

    图表设计思路（为什么选择这一类型的图表展示这些数据）
    图表类型
    图表的布局（如果图表在仪表板中占据了过大或过小的部分，需要说明这样布局的理由）
    图表的图例（例如颜色、形状、大小等代表什么变量）
    诸如此类的信息。目前的设计部分还不完全符合此要求。请在下次提交中完善报告的“设计”部分。
 - 修改：完善了设计部分的内容。
 
- 审阅意见：故事点1颜色无图例，请补充。其次请使用合理方法使得观众能清楚区别折线和条柱分别代表的变量是什么；
     故事点3颜色无图例，请补充；
     故事点4热力图中方块大小无图例，请补充。
 - 修改：增加图例，并修改别名等，以便使观众更清晰地理解其含义。
 
- 审阅意见：你需要根据每次审阅意见持续更新反馈部分。也就是说，在下次提交时，你应当将本次审阅内容作为反馈，记录在下次提交的“反馈部分”。

    同时，针对反馈的记录，一方面，你需要尽量具体地指出他人的反馈意见（最好是针对特定的可视化或文字说明）；另一方面，你必须完整说明针对他人的反馈，你对可视化做了哪些改进，如果未根据反馈修改，你需要说明理由。请按照此原则持续更新反馈部分。这里提供一个反馈部分的示例，请按照示例更新此部分：

 - 修改：按照反馈要求，复制了第一次的反馈意见和修改内容。
=======
朋友甲：  
- 周末/非周末骑行数量并非1/3，而是8月的周末/非周末天数为1/3，因而饼图混淆概念；
- 尽展示了一个仪表盘，而非一个故事集；  

朋友乙：  
- 可以在骑行数量中对工作日/周末进行颜色标注，从而更多唯独展现；
>>>>>>> cd078070df9781a17bb286d8b627717a8e15bcb3


### 资源
- 参考资源：https://public.tableau.com/profile/ting.wang#!/vizhome/MobikeProject/MobikeStory4_0
