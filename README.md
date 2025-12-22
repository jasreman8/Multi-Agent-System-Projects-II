# Multi-Agent-System-Projects-II

Project 1: Built a reflection-pattern multi-agent workflow in LangGraph for automated ad copy generation and approval:
- Implemented Ad Copywriter agent to draft and revise copy using product feature context
- Implemented Compliance Reviewer agent to validate drafts against rule-based checks and provide actionable feedback
- Added decision node + revision loop (Draft → Review → Revise) until compliance approval is achieved
- Defined shared workflow state to track product, audience, draft copy, feedback, and approval status across turns

Project 2: Built a financial research ReAct-style agent with custom tools (stock price + company info) and web search
- Implemented automated test case generation, capturing final responses and full tool call traces
- Created realistic evaluation scenarios with expected tool usage per query
- Applied DeepEval metrics, including TaskCompletionMetric and ToolCorrectnessMetric to score agent behavior
- Added notebook workflow demonstrating end-to-end agent evaluation: build → test-case capture → metric scoring → analysis

