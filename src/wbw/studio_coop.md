# 协作
通过消息功能，实现翻译的网络协作。

只有具备**共享属性**的文档，才可以发消息。

逐词译、译文的每次修改，都会发消息给协作者

数据合并逻辑：
- 用户数据大体包括四种状态
  - 用户**手动**修改
  - 他人**消息**推动
  - 机器**自动**匹配
  - 新经文中的**未填充**部分
- 覆盖逻辑
  - 手动>消息>自动>未填充
-  未能覆盖则在改数据位置上显示<span style="color:#f9468f">消息数量</span>提示