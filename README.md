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

Project 3: Implemented a modular multi-agent travel planner in LangGraph for automated, personalized trip planning:
- Built Destination Recommender using the Reflection pattern (Destination-Suggester ↔ Destination-Reviewer loop)
- Built Itinerary Planner using the Supervisor pattern, orchestrating Hotel, Local Guide, Trip Planning, and Language Assistance agents
- Added specialized tool functions for weather suitability, ticket availability, language compatibility, and local event risk checks (TavilySearch-backed)
- Enforced destination constraints (avoid previously rejected destinations, single-destination recommendation per iteration)
- Integrated agent evaluation using DeepEval metrics:
  - TaskCompletionMetric for preference alignment of destination recommendation
  - ToolCorrectnessMetric to verify correct tool usage across the workflow
