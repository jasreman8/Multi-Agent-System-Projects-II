# Multi-Agent-System-Projects-II

Project 1: Built a reflection-pattern multi-agent workflow in LangGraph for automated ad copy generation and approval:
- Implemented Ad Copywriter agent to draft and revise copy using product feature context
- Implemented Compliance Reviewer agent to validate drafts against rule-based checks and provide actionable feedback
- Added decision node + revision loop (Draft → Review → Revise) until compliance approval is achieved
- Defined shared workflow state to track product, audience, draft copy, feedback, and approval status across turns
