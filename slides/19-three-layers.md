---
layout: default
---

# Three Layers of Context Engineering

<div class="three-layers-container">
  <div class="layer layer-conversation">
    <div class="layer-icon">
      <uim-comment-alt class="text-5xl text-blue-400"/>
    </div>
    <div class="layer-content">
      <h3>Conversation Memory</h3>
      <p>Systematic thinking and organized problem analysis</p>
    </div>
  </div>
  
  <div class="layer layer-process">
    <div class="layer-icon">
      <uim-process class="text-5xl text-green-400"/>
    </div>
    <div class="layer-content">
      <h3>Process Memory</h3>
      <p>Phase-aware development plans and progress tracking</p>
    </div>
  </div>
  
  <div class="layer layer-longterm">
    <div class="layer-icon">
      <uim-document-layout-left class="text-5xl text-purple-400"/>
    </div>
    <div class="layer-content">
      <h3>Long-term Memory</h3>
      <p>Requirements, Documentation, RAG</p>
    </div>
  </div>
</div>

<style scoped>
.three-layers-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  max-width: 800px;
  margin: 2rem auto;
  padding: 2rem;
}

.layer {
  display: flex;
  align-items: center;
  padding: 1.5rem 2rem;
  border-radius: 12px;
  backdrop-filter: blur(10px);
  border: 2px solid;
  transition: transform 0.2s ease;
}

.layer:hover {
  transform: translateX(10px);
}

.layer-conversation {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.2), rgba(147, 51, 234, 0.2));
  border-color: rgba(59, 130, 246, 0.4);
}

.layer-process {
  background: linear-gradient(135deg, rgba(34, 197, 94, 0.2), rgba(59, 130, 246, 0.2));
  border-color: rgba(34, 197, 94, 0.4);
}

.layer-longterm {
  background: linear-gradient(135deg, rgba(147, 51, 234, 0.2), rgba(168, 85, 247, 0.2));
  border-color: rgba(147, 51, 234, 0.4);
}

.layer-icon {
  margin-right: 2rem;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.layer-content h3 {
  margin: 0 0 0.5rem 0;
  font-size: 1.5rem;
  font-weight: 600;
}

.layer-content p {
  margin: 0;
  font-size: 1rem;
  opacity: 0.8;
}
</style>

<!--

**Speaker Notes:**
Main message: Three-layer framework provides practical structure for maintaining and delivering clear context to AI systems

- Three layers
- Practical framework
- Clear context

*Transition: This leads us to a fundamental shift in how we think about engineering.*

...

Once you establish clear thinking, you need a practical framework to maintain and provide that clarity. This is the three-layer context engineering approach I developed while building workflows. 

Layer 1 is Rich Conversation Context - organizing your thinking systematically, asking the right questions, clarifying requirements methodically. 

Layer 2 is Process Memory - phase-aware development plans that track what phase you're in, what decisions you've made, what's been completed. 

Layer 3 is Long-term Memory - requirements, architecture, and design documents that preserve your thinking across conversations and sessions. This may as well be captured outside the system, e. g. in knowledge databases connected via RAG. 

These three layers provide the context AI needs to transform from chaotic assistant to capable execution partner.

-->
