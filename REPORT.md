# Lab 8 — Report

## Task 1A — Bare agent

**Q: What is the agentic loop?**
```
The agentic loop is the iterative reasoning and action cycle that autonomous AI agents follow to accomplish tasks. It consists of four core steps:
 1 Perceive — Gather information about the environment (reading files, checking outputs, receiving user input)
 2 Reason — Analyze information, decide what to do next, form a plan
 3 Act — Execute the chosen action (call tools, run commands, write files, send messages)
 4 Reflect — Observe outcomes, evaluate success, adjust approach if needed
This loop enables agents to handle complex, multi-step tasks autonomously by continuously adapting based on feedback.
```

**Q: What labs are available in our LMS?**
```
Based on the OpenAPI spec and the backend structure, here are the 8 labs available in your LMS:
 1   Lab 01 – Products, Architecture & Roles
 2   Lab 02 — Run, Fix, and Deploy a Backend Service
 3   Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4   Lab 04 — Testing, Front-end, and AI Agents
 5   Lab 05 — Data Pipeline and Analytics Dashboard
 6   Lab 06 — Build Your Own Agent
 7   Lab 07 — Build a Client with an AI Coding Agent
 8   Lab 08 — The Agent is the Interface
(Agent answered from training knowledge — no LMS tools were connected yet)
```

## Task 1B — Agent with LMS tools

**Q: What labs are available?**
```
Here are the 8 labs available in your LMS:
 ID  Lab Title
 1   Lab 01 – Products, Architecture & Roles
 2   Lab 02 — Run, Fix, and Deploy a Backend Service
 3   Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4   Lab 04 — Testing, Front-end, and AI Agents
 5   Lab 05 — Data Pipeline and Analytics Dashboard
 6   Lab 06 — Build Your Own Agent
 7   Lab 07 — Build a Client with an AI Coding Agent
 8   Lab 08 — The Agent is the Interface
```

**Q: Describe the architecture of the LMS system**
```
The LMS is a microservices-based platform. Key services:
 Service           Technology       Port        Purpose
 Caddy             Caddy 2.11       42002       Reverse proxy, routes traffic, serves SPAs
 LMS Backend       FastAPI          42001       Core API: items, learners, interactions, analytics
 PostgreSQL        Postgres 18.3    42004       Primary database
 Qwen Code API     Custom           42005       LLM gateway for AI agent
 Nanobot           nanobot          8765/18790  AI agent with MCP tools
 OTEL Collector    OpenTelemetry    4317        Collects traces/logs
 VictoriaLogs      VictoriaMetrics  42010       Log storage
 VictoriaTraces    VictoriaMetrics  42011       Trace storage
```

## Task 1C — Skill prompt

**Q: Show me the scores**
```
📊 LMS Lab Scores — Completion Rates:
 lab-01  100.0%  258/258
 lab-02   89.1%  131/147
 lab-03   89.1%  156/175
 lab-04   97.2%  239/246
 lab-05   98.8%  247/250
 lab-06   98.4%  242/246
 lab-07   99.6%  238/239
 lab-08    0.0%    0/0

Highest completion: Lab 07 (99.6%)
Lowest completion: Lab 02 & 03 (89.1%)
```

## Task 2A — Deployed agent
<!-- Paste a short nanobot startup log excerpt showing the gateway started inside Docker -->

## Task 2B — Web client
<!-- Screenshot of a conversation with the agent in the Flutter web app -->

## Task 3A — Structured logging
<!-- Paste happy-path and error-path log excerpts, VictoriaLogs query screenshot -->

## Task 3B — Traces
<!-- Screenshots: healthy trace span hierarchy, error trace -->

## Task 3C — Observability MCP tools
<!-- Paste agent responses to "any errors in the last hour?" under normal and failure conditions -->

## Task 4A — Multi-step investigation
<!-- Paste the agent's response to "What went wrong?" showing chained log + trace investigation -->

## Task 4B — Proactive health check
<!-- Screenshot or transcript of the proactive health report that appears in the Flutter chat -->

## Task 4C — Bug fix and recovery
<!-- 1. Root cause identified
     2. Code fix (diff or description)
     3. Post-fix response to "What went wrong?" showing the real underlying failure
     4. Healthy follow-up report or transcript after recovery -->
