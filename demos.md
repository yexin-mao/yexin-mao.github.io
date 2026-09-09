---
title: "Project Demos | Yexin Mao"
permalink: /demos/
layout: single
author_profile: false
classes: wide
---

<style>
.demo-shell {
  --ink: #171717;
  --muted: #66645f;
  --line: #dedbd3;
  --accent: #315fe8;
  max-width: 1120px;
  margin: 0 auto;
  color: var(--ink);
}
.demo-intro {
  display: grid;
  grid-template-columns: minmax(0, 1fr) auto;
  align-items: end;
  gap: 1.5rem;
  padding: 1.2rem 0 2rem;
  border-bottom: 1px solid var(--line);
}
.demo-kicker {
  margin-bottom: .45rem;
  color: var(--accent);
  font-size: .76rem;
  font-weight: 800;
  letter-spacing: .12em;
  text-transform: uppercase;
}
.demo-intro h1 {
  margin: 0;
  font-size: clamp(2rem, 5vw, 4rem);
  line-height: 1.02;
}
.demo-intro p {
  max-width: 720px;
  margin: .85rem 0 0;
  color: var(--muted);
  font-size: 1rem;
}
.demo-back {
  white-space: nowrap;
  font-weight: 700;
  text-decoration: none !important;
}
.demo-item {
  display: grid;
  grid-template-columns: minmax(0, 1.65fr) minmax(260px, .75fr);
  gap: 1.6rem;
  padding: 2.2rem 0;
  border-bottom: 1px solid var(--line);
  scroll-margin-top: 2rem;
}
.demo-player {
  overflow: hidden;
  border: 1px solid #d7d3ca;
  border-radius: 16px;
  background: #111;
  box-shadow: 0 18px 48px rgba(34, 31, 25, .12);
}
.demo-player video {
  display: block;
  width: 100%;
  aspect-ratio: 16 / 9;
  background: #111;
}
.demo-index {
  color: var(--accent);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  font-weight: 700;
  letter-spacing: .08em;
}
.demo-copy h2 {
  margin: .35rem 0 .25rem;
  font-size: 1.7rem;
}
.demo-subtitle {
  margin: 0 0 1rem;
  color: var(--muted);
}
.demo-copy ul {
  margin: 1rem 0 1.25rem;
  padding-left: 1.1rem;
}
.demo-copy li { margin-bottom: .45rem; }
.demo-actions {
  display: flex;
  flex-wrap: wrap;
  gap: .7rem;
}
.demo-button {
  display: inline-block;
  padding: .62rem .9rem;
  border: 1px solid #c9c6bf;
  border-radius: 999px;
  font-size: .88rem;
  font-weight: 700;
  text-decoration: none !important;
}
.demo-button.primary {
  border-color: var(--ink);
  background: var(--ink);
  color: white !important;
}
.demo-note {
  margin: 1.25rem 0 0;
  color: var(--muted);
  font-size: .82rem;
}
@media (max-width: 820px) {
  .demo-intro,
  .demo-item { grid-template-columns: 1fr; }
  .demo-back { justify-self: start; }
}
</style>

<div class="demo-shell">
  <header class="demo-intro">
    <div>
      <div class="demo-kicker">Selected work · 中文讲解</div>
      <h1>Project demos</h1>
      <p>两个完整项目演示：先看真实工作流与结果，再进入仓库检查实现、测试和评测证据。</p>
    </div>
    <a class="demo-back" href="/">← Back to portfolio</a>
  </header>

  <section class="demo-item" id="code-agent">
    <div class="demo-player">
      <video controls preload="metadata" playsinline poster="/images/demos/code-agent-v34.jpg">
        <source src="/assets/videos/code-agent-demo-v34-zh.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="demo-copy">
      <div class="demo-index">01 / CODE AGENT · 11:05</div>
      <h2>本地编码智能体</h2>
      <p class="demo-subtitle">从最小 Agent 循环到可恢复、可审查的仓库级交付。</p>
      <ul>
        <li>代码调查、修改、测试与审查闭环</li>
        <li>结构化计划与多智能体并行探索</li>
        <li>权限确认、失败恢复与隔离交付</li>
        <li>SWE-bench Verified 真实模型评测</li>
      </ul>
      <div class="demo-actions">
        <a class="demo-button primary" href="https://github.com/yexin-mao/coding-agent-from-scratch">View source</a>
        <a class="demo-button" href="/assets/videos/code-agent-demo-v34-zh.mp4">Open video</a>
      </div>
    </div>
  </section>

  <section class="demo-item" id="minibrain">
    <div class="demo-player">
      <video controls preload="metadata" playsinline poster="/images/demos/minibrain-v20.jpg">
        <source src="/assets/videos/minibrain-demo-v20-zh.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="demo-copy">
      <div class="demo-index">02 / MINIBRAIN · 07:10</div>
      <h2>企业知识库问答与 LLM Wiki</h2>
      <p class="demo-subtitle">让不同的数据进入正确的检索链路，并交付可验证答案。</p>
      <ul>
        <li>文档 Vector RAG 与表格 Table RAG</li>
        <li>混合检索、重排序与 parent-aware 去重</li>
        <li>Evidence ID 引用校验和安全拒答</li>
        <li>多用户权限、可观测记录与回归评测</li>
      </ul>
      <div class="demo-actions">
        <a class="demo-button primary" href="https://github.com/yexin-mao/minibrain">View source</a>
        <a class="demo-button" href="/assets/videos/minibrain-demo-v20-zh.mp4">Open video</a>
      </div>
    </div>
  </section>

  <p class="demo-note">视频采用 H.264 / AAC 编码并针对网页顺序播放优化；移动端建议使用横屏观看。</p>
</div>
