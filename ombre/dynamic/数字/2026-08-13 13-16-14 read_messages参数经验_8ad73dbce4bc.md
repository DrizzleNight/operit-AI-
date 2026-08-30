---
activation_count: 0
arousal: 0.3
created: '2026-08-13T13:16:14'
domain:
- 数字
id: 8ad73dbce4bc
importance: 6
last_active: '2026-08-13T13:16:14'
name: 2026-08-13 13-16-14 read_messages参数经验
tags:
- read_messages
- extended_chat
- 参数配置
- 分页读取
- Operit
type: dynamic
valence: 0.5
---

在Operit记忆库的`extended_chat`工具包中，`read_messages`调用使用`order: "asc"`从最早消息读取时，默认limit值20不足以覆盖长对话（如817条消息）中的关键起始点。需配合足够大的limit值（如500）或分页偏移量多次调用才能完整覆盖。在极长对话中精准查找特定消息文本时，可考虑结合`list_chats`的`messagesFilter`按内容搜索功能。