# 笔记

先把相关概念拎出来
Harness
Loop
Agent Protocol ->  Thread(Session) / Run(Task) / Event / Artifact / Checkpoint 


| 对象               | 人话解释             | 它回答的问题              |
| :--------------- | :--------------- | :------------------ |
| Thread / Session | 一段长期上下文          | 这是谁的哪段任务？           |
| Run/ Task        | 一次具体执行（某个会话中的问题） | 这次具体跑了什么？           |
| Step             | 执行中的一个可观测步骤      | 哪一步调用了模型、工具或子Agent？ |
| Event            | 执行过程中的进展变化       | 现在发生了什么？            |
| Artifact         | Agent产出的正式结果     | 结果在哪里，由哪次执行产生？      |
| Checkpoint       | 可以恢复的执行快照        | 失败或中断后从哪里继续？        |



Runtime Loop ：谁拥有主循环，控制流被放在哪种运行时容器里。 
- **ReAct**可以看成某个最小Loop中的执行步骤
- **Plan-and-Execute** 的关键是把 Plan / Todo / Step / Progress 提升为显式状态。
- **Conversation-style coordination** 的关键是把 Participant / Message / Route / Handoff / Speaker 提升为显式状态。