---
license: cc-by-nc-sa-4.0
task_categories:
- text-classification
language:
- en
pretty_name: 豆包大模型测试
---

# 豆包大模型测试

本需求仅描述“豆包大模型测试”，未提供具体测试类型（如对齐评测、鲁棒性、安全红队、RAG评测、工具调用评测等）、测试数据形态、样例规模、交付标准、时间与预算等信息。

建议在需求澄清中补充：
1) 测试目标：功能正确性/性能指标、安全与合规/鲁棒性/幻觉与事实一致性/RAG与工具调用等；
2) 测试数据类型：文本为主还是多模态；是否包含恶意/越狱/Prompt Injection；是否需要标注的评测集；
3) 数据规模：总量与样例数（及单位）；
4) 交付标准：包含通过率/指标阈值/报告模板等；
5) 优先级、交付日期、预算与排他性与否。

## Technical Specifications

| Field | Type | Description |
| :---  | :---  | :--- |
| test_case_input | string | 一条测试用例的原始输入文本（用户提示/任务描述/上下文等）。 |
| test_case_language | string | 对测试输入的语言识别结果（如 zh/en/其他），用于按语言维度切分统计。 |
| test_case_domain_hint | string | 从测试输入推断的领域或意图线索（例如客服、代码生成、总结、对话、知识问答等），用于归类与报告汇总。 |
| test_case_length_chars | integer | 测试输入文本的字符数统计，用于粗粒度长度分布分析与难度分层。 |
| test_case_normalized_text | string | 对原始输入进行规范化后的文本（例如去除多余空白、统一换行、可选清洗特殊字符），用于一致性评测与复现实验。 |
| test_case_has_jailbreak_risk | boolean | 对测试文本中疑似越狱、提示注入（Prompt Injection）等风险的粗粒度标记，供安全/鲁棒性评测分组使用。 |

## Compliance Statement

<table>
  <tr><td>Authorization Type</td><td>CC-BY-NC-SA 4.0 (Attribution–NonCommercial–ShareAlike)</td></tr>
  <tr><td>Commercial Use</td><td>Requires exclusive subscription or authorization contract (monthly or per-invocation charging)</td></tr>
  <tr><td>Privacy and Anonymization</td><td>No PII, no real company names, simulated scenarios follow industry standards</td></tr>
  <tr><td>Compliance System</td><td>Compliant with China's Data Security Law / EU GDPR / supports enterprise data access logs</td></tr>
</table>


## Source & Contact

contact@mobiusi.com

