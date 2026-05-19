---
layout: image-lower-third
image: /10-agent-workflow.png
---

# The Agent Approach

**Best for:** Workflows with deliberately diverse roles, different angles, different tools

<!--
**Speaker Notes:**
Main message: Agents aren't about compensating for model limitations — they're about deliberately introducing diversity of perspective and tooling

- Deliberate role separation: critic, implementer, tester
- Different tools per agent: search, code execution, DB queries
- ⚠️ Coordination overhead — overkill for simple tasks
- ⚠️ Context sharing between agents is non-trivial
- ⚠️ Parallel execution is a two-sided sword

*Transition: When you already know exactly what to look at, IDE integration is more direct.*

...

**Reader Notes:**

The agent approach is often misunderstood as a workaround for model limitations. Today, it's better understood as a deliberate architectural choice: you *want* different perspectives.

A critic agent and an implementer agent will produce better results than a single agent asked to "be critical and then implement" — because the role separation is structural, not just instructional. Similarly, agents with different tool access (web search, code execution, database queries) can work in parallel on different aspects of a problem.

The key word is *deliberately*: you're not splitting work because the model can't handle it all — you're splitting it because different roles genuinely benefit from different contexts and constraints.

The coordination overhead is real, so agents are overkill for simple tasks. But for complex workflows where diverse perspectives add value, they're the right tool.
-->
