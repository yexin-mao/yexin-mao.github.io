---
title: "Yexin Mao | AI Agent Engineer"
permalink: /
author_profile: true
---

<style>
.agent-hero {
  padding: 2.2rem 0 1.4rem;
  border-bottom: 1px solid #e5e7eb;
}
.agent-eyebrow {
  color: #2563eb;
  font-weight: 700;
  letter-spacing: .04em;
  text-transform: uppercase;
  font-size: .78rem;
}
.agent-hero h1 {
  margin: .35rem 0 .65rem;
  font-size: clamp(2rem, 4vw, 3.2rem);
  line-height: 1.08;
}
.agent-lead {
  max-width: 820px;
  font-size: 1.05rem;
  color: #374151;
}
.agent-actions {
  display: flex;
  flex-wrap: wrap;
  gap: .75rem;
  margin-top: 1.25rem;
}
.agent-btn {
  display: inline-block;
  padding: .68rem .95rem;
  border-radius: 999px;
  font-weight: 700;
  text-decoration: none !important;
  border: 1px solid #d1d5db;
}
.agent-btn.primary {
  background: #111827;
  color: white !important;
  border-color: #111827;
}
.agent-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1rem;
  margin: 1.2rem 0 2rem;
}
.agent-card {
  border: 1px solid #e5e7eb;
  border-radius: 18px;
  padding: 1.15rem;
  background: linear-gradient(180deg, #ffffff 0%, #f8fafc 100%);
  box-shadow: 0 10px 30px rgba(15, 23, 42, .06);
}
.agent-card h3 { margin-top: 0; }
.agent-card-media {
  display: block;
  position: relative;
  margin: -1.15rem -1.15rem 1rem;
  overflow: hidden;
  border-radius: 18px 18px 0 0;
  background: #111827;
}
.agent-card-media img {
  display: block;
  width: 100%;
  aspect-ratio: 16 / 9;
  object-fit: cover;
  transition: transform .2s ease, opacity .2s ease;
}
.agent-card-media:hover img {
  transform: scale(1.015);
  opacity: .86;
}
.agent-play {
  position: absolute;
  left: 1rem;
  bottom: 1rem;
  padding: .48rem .72rem;
  border-radius: 999px;
  background: rgba(17, 24, 39, .88);
  color: #fff;
  font-size: .78rem;
  font-weight: 700;
}
.agent-card-actions {
  display: flex;
  flex-wrap: wrap;
  gap: .85rem;
  margin-bottom: 0;
  font-weight: 700;
}
.agent-tag {
  display: inline-block;
  margin: .15rem .2rem .15rem 0;
  padding: .24rem .5rem;
  border-radius: 999px;
  background: #eff6ff;
  color: #1d4ed8;
  font-size: .78rem;
  font-weight: 700;
}
.agent-muted { color: #6b7280; }
.agent-section { margin-top: 2rem; }
.agent-list li { margin-bottom: .45rem; }
.agent-status {
  padding: .85rem 1rem;
  border-left: 4px solid #2563eb;
  background: #eff6ff;
  border-radius: 10px;
}
</style>

<div class="agent-hero">
  <div class="agent-eyebrow">AI Agent Engineer / Applied AI Engineer</div>
  <h1>Building reliable AI agents that retrieve evidence, use tools, and complete multi-step work.</h1>
  <p class="agent-lead">
    I am Yexin Mao, a Computer Vision and Machine Learning graduate now focused on reliable AI Agent and RAG systems. My two core projects cover autonomous repository work and evidence-grounded enterprise knowledge retrieval, with reproducible tests and evaluations.
  </p>
  <div class="agent-actions">
    <a class="agent-btn primary" href="/demos/">Watch Project Demos</a>
    <a class="agent-btn" href="/projects/">View Projects</a>
    <a class="agent-btn" href="https://github.com/yexin-mao">GitHub</a>
  </div>
</div>

## Featured AI Agent Projects

<div class="agent-grid">
  <div class="agent-card">
    <a class="agent-card-media" href="/demos/#code-agent" aria-label="Watch the Code Agent demo">
      <img src="/images/demos/code-agent-v34.jpg" alt="Code Agent demo preview">
      <span class="agent-play">▶ Watch demo · 11:05</span>
    </a>
    <h3>Code Agent</h3>
    <p class="agent-muted">A reliable local coding agent for repository-level work.</p>
    <p>
      Investigates, edits, tests, reviews, and delivers code through a recoverable workflow, with structured planning, multi-agent exploration, approval boundaries, and SWE-bench evaluation.
    </p>
    <p>
      <span class="agent-tag">LangGraph</span>
      <span class="agent-tag">Tool Calling</span>
      <span class="agent-tag">Multi-Agent</span>
      <span class="agent-tag">SWE-bench</span>
    </p>
    <p class="agent-card-actions"><a href="/demos/#code-agent">Watch video →</a><a href="https://github.com/yexin-mao/coding-agent-from-scratch">Source code →</a></p>
  </div>

  <div class="agent-card">
    <a class="agent-card-media" href="/demos/#minibrain" aria-label="Watch the Minibrain demo">
      <img src="/images/demos/minibrain-v20.jpg" alt="Minibrain demo preview">
      <span class="agent-play">▶ Watch demo · 07:10</span>
    </a>
    <h3>Minibrain</h3>
    <p class="agent-muted">Enterprise knowledge QA and versioned LLM Wiki.</p>
    <p>
      Routes questions across document Vector RAG and structured Table RAG, returns evidence-verified answers, and turns source documents into maintainable, versioned wiki pages.
    </p>
    <p>
      <span class="agent-tag">Hybrid RAG</span>
      <span class="agent-tag">LangGraph</span>
      <span class="agent-tag">Evidence</span>
      <span class="agent-tag">Evaluation</span>
    </p>
    <p class="agent-card-actions"><a href="/demos/#minibrain">Watch video →</a><a href="https://github.com/yexin-mao/minibrain">Source code →</a></p>
  </div>
</div>

<div class="agent-status">
  <strong>Two narrated demos are available:</strong> watch the complete workflows in the browser, then open the corresponding repository for implementation details and evaluation evidence.
</div>

<div class="agent-section">

## What I want to demonstrate

<ul class="agent-list">
  <li><strong>AI-native product thinking:</strong> agents as workflows, not one-shot chatbot responses.</li>
  <li><strong>Reliable RAG:</strong> hybrid retrieval, evidence binding, permission-aware access, and regression evaluation.</li>
  <li><strong>Coding agent engineering:</strong> planning, state, tools, retries, approvals, review, and isolated delivery.</li>
  <li><strong>Production readiness:</strong> GitHub repos, readable documentation, web demos, and measurable task outcomes.</li>
</ul>

</div>
