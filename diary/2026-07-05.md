# 2026-07-05 学习记录

## 今天做了什么
- 修复了 Agent 工具调用时参数为空的 Bug
- 读了 DefaultReActAgent.run() 的迭代控制逻辑

## 学到了什么
1. DefaultReActAgent 的 tool_calls 会通过 filterValidToolCalls() 
   过滤掉 name 或 arguments 为空的调用，防止空指针
2. 项目的 SSE 事件协议有 5 种事件：start / output / status / end / error

## 遇到的坑
- 数据库连接失败 → 原来是 Redis 没启动，SaToken 初始化报错
  解决：先启动 Redis 再启动后端

## 明天计划
- 看完 MultiAgentUtil 的多 Agent 调度逻辑
- 开始做"文章收藏"功能