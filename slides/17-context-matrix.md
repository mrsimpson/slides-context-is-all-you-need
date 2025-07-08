---
layout: default
---

# Context Relevance by Phase

<div class="mt-8">

| Information Type | Project Start | Implementation | Debugging |
|------------------|---------------|----------------|-----------|
| Requirements     | <div class="i-uim-check text-green-500 inline"></div> Critical   | <div class="i-uim-times text-red-500 inline"></div> Noise      | <div class="i-uim-times text-red-500 inline"></div> Noise  |
| Code Files       | <div class="i-uim-times text-red-500 inline"></div> Noise      | <div class="i-uim-check text-green-500 inline"></div> Critical   | <div class="i-uim-check text-green-500 inline"></div> Critical |
| Error Logs       | <div class="i-uim-times text-red-500 inline"></div> Noise      | <div class="i-uim-times text-red-500 inline"></div> Noise      | <div class="i-uim-check text-green-500 inline"></div> Critical |
| Architecture     | <div class="i-uim-check text-green-500 inline"></div> Critical   | <div class="i-uim-exclamation-triangle text-yellow-500 inline"></div> Sometimes  | <div class="i-uim-times text-red-500 inline"></div> Noise  |

</div>

<!--
This matrix illustrates the core principle. The same piece of information can be critical in one phase and pure noise in another.

Requirements are critical when starting a project but become noise when you're deep in debugging. Error logs are essential for debugging but irrelevant when you're planning architecture.

Traditional approaches either try to provide everything (information overload) or make humans decide what's relevant (cognitive overload). Context Engineering provides the right information for the current phase.
-->
