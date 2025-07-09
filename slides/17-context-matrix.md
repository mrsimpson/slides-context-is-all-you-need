---
layout: default
---

# Context Relevance by Phase

<div class="mt-8">

| Information Type | Project Start | Implementation | Debugging |
|------------------|---------------|----------------|-----------|
| Requirements     | <uim-check class="text-green-500 inline"/> Critical   | <uim-times-circle class="text-red-500 inline"/> Noise      | <uim-times-circle class="text-red-500 inline"/> Noise  |
| Code Files       | <uim-times-circle class="text-red-500 inline"/> Noise      | <uim-check class="text-green-500 inline"/> Critical   | <uim-check class="text-green-500 inline"/> Critical |
| Error Logs       | <uim-times-circle class="text-red-500 inline"/> Noise      | <uim-times-circle class="text-red-500 inline"/> Noise      | <uim-check class="text-green-500 inline"/> Critical |
| Architecture     | <uim-check class="text-green-500 inline"/> Critical   | <uim-exclamation-triangle class="text-yellow-500 inline"/> Sometimes  | <uim-times-circle class="text-red-500 inline"/> Noise  |

</div>

<!--
This matrix illustrates the core principle. The same piece of information can be critical in one phase and pure noise in another.

Requirements are critical when starting a project but become noise when you're deep in debugging. Error logs are essential for debugging but irrelevant when you're planning architecture.

Traditional approaches either try to provide everything (information overload) or make humans decide what's relevant (cognitive overload). Context Engineering provides the right information for the current phase.
-->
