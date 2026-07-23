# 通知模板 — 运行成功
#
# 可用变量（使用 {变量名} 引用）：
#   {status}               — 状态文本（SUCCESS / FAILED）
#   {timestamp}            — 运行时间戳
#   {total_fetched}        — 抓取论文总数
#   {total_qualified}      — 及格论文总数
#   {total_analyzed}       — 深度分析论文总数
#   {source_summary}       — 各数据源统计（已格式化）
#   {report_list}          — 报告路径列表（已格式化）
#   {top_papers}           — Top-N 论文列表（已格式化）
#   {error_message}        — 错误信息（成功时为空）
#   {token_usage_section}  — Token 消耗统计（已格式化，关闭追踪时为空）
#
# 企业微信 Markdown 支持说明：
#   支持：# 标题、**加粗**、[链接](url)、`代码`、> 引用
#   支持：<font color="info">绿色</font> <font color="warning">橙色</font> <font color="comment">灰色</font>
#   不支持：表格、图片、有序列表
#   限制：总内容不超过 4096 字节
#
# 修改此文件即可自定义成功通知的样式和内容。

## 📚 文献日报

{timestamp}

本次共抓取 **{total_fetched}** 篇论文，筛选出 **{total_qualified}** 篇相关论文。

---

{top_papers}
