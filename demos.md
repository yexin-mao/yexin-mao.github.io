---
title: "Project Demos"
permalink: /demos/
layout: single
author_profile: false
classes: wide
---

<style>
body,
.masthead,
.page__footer {
  background: #f7f7f3;
}
.page__title { display: none; }
.page {
  float: none !important;
  width: 100% !important;
  padding-right: 0 !important;
}
.page__inner-wrap {
  max-width: 1160px;
  margin: 0 auto;
}
.page__content { margin-top: .5rem; }
.demo-shell {
  --paper: #f7f7f3;
  --ink: #101113;
  --muted: #73757a;
  --rule: #d9dadd;
  --blue: #315cf5;
  max-width: 1160px;
  margin: 0 auto;
  color: var(--ink);
  font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Hiragino Sans GB", sans-serif;
}
.demo-intro {
  padding: 1.1rem 0 3.5rem;
}
.demo-topline,
.demo-item-head {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 1.5rem;
  padding-bottom: .85rem;
  border-bottom: 1px solid var(--rule);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .8rem;
  letter-spacing: .055em;
  text-transform: uppercase;
}
.demo-label {
  display: block;
  color: var(--ink);
}
.demo-kicker {
  display: block;
  margin-top: .22rem;
  color: var(--blue);
}
.demo-back {
  color: var(--ink) !important;
  font-weight: 650;
  text-decoration: none !important;
  white-space: nowrap;
}
.demo-hero {
  display: grid;
  grid-template-columns: minmax(190px, .72fr) minmax(0, 2.1fr);
  gap: clamp(2rem, 7vw, 7rem);
  align-items: end;
  padding-top: 3rem;
}
.demo-count strong {
  display: block;
  color: var(--blue);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: clamp(5rem, 11vw, 8.2rem);
  font-weight: 400;
  line-height: .82;
  letter-spacing: -.08em;
}
.demo-count span {
  display: block;
  margin-top: .95rem;
  color: var(--muted);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .77rem;
  letter-spacing: .09em;
}
.demo-hero h1 {
  margin: 0;
  color: var(--ink);
  font-size: clamp(2.25rem, 5.4vw, 4.35rem);
  font-weight: 650;
  line-height: 1.16;
  letter-spacing: -.045em;
}
.demo-hero p {
  max-width: 690px;
  margin: 1.15rem 0 0;
  color: var(--muted);
  font-size: 1rem;
  line-height: 1.8;
}
.demo-item {
  padding: 1.25rem 0 3.8rem;
  scroll-margin-top: 2rem;
}
.demo-item + .demo-item {
  padding-top: 1.25rem;
}
.demo-item-head {
  margin-bottom: 1.25rem;
}
.demo-item-head strong {
  color: var(--blue);
  font-weight: 500;
}
.demo-item-head span:last-child {
  color: var(--muted);
}
.demo-player {
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border: 1px solid var(--rule);
  border-radius: 3px;
  background: #101113;
}
.demo-player video {
  display: block;
  width: 100%;
  height: 100% !important;
  object-fit: cover;
  background: #101113;
}
.demo-copy {
  display: grid;
  grid-template-columns: minmax(230px, .8fr) minmax(0, 1.35fr) auto;
  gap: clamp(1.5rem, 4vw, 4rem);
  align-items: start;
  padding-top: 1.55rem;
}
.demo-copy h2 {
  margin: 0;
  color: var(--ink);
  font-size: clamp(1.45rem, 2.8vw, 2rem);
  font-weight: 650;
  line-height: 1.3;
  letter-spacing: -.025em;
}
.demo-subtitle {
  margin: .58rem 0 0;
  color: var(--muted);
  font-size: .98rem;
  line-height: 1.7;
}
.demo-copy ul {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0 1.75rem;
  margin: 0;
  padding: 0;
  list-style: none;
}
.demo-copy li {
  position: relative;
  min-height: 3.1rem;
  padding: .18rem 0 .75rem 1rem;
  border-bottom: 1px solid var(--rule);
  color: #37383b;
  font-size: .92rem;
  line-height: 1.55;
}
.demo-copy li::before {
  position: absolute;
  top: .78em;
  left: 0;
  width: 5px;
  height: 2px;
  background: var(--blue);
  content: "";
}
.demo-actions {
  display: grid;
  gap: .75rem;
  min-width: 7.5rem;
}
.demo-button {
  display: inline-flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
  padding: .3rem 0 .48rem;
  border-bottom: 1px solid var(--rule);
  color: var(--ink) !important;
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  font-weight: 600;
  letter-spacing: .02em;
  text-decoration: none !important;
}
.demo-button::after {
  color: var(--blue);
  content: "↗";
}
.demo-button.primary {
  border-bottom-color: var(--blue);
  color: var(--blue) !important;
}
.demo-note {
  margin: -1rem 0 0;
  padding: 1rem 0 0;
  border-top: 1px solid var(--rule);
  color: var(--muted);
  font-size: .82rem;
  line-height: 1.6;
}
.demo-back:hover,
.demo-button:hover {
  color: var(--blue) !important;
}
.demo-back:focus-visible,
.demo-button:focus-visible,
.demo-player video:focus-visible {
  outline: 2px solid var(--blue);
  outline-offset: 4px;
}
@media (max-width: 900px) {
  .demo-copy {
    grid-template-columns: 1fr 1.25fr;
  }
  .demo-actions {
    grid-column: 1 / -1;
    grid-template-columns: repeat(2, minmax(0, 9rem));
  }
}
@media (max-width: 680px) {
  .demo-intro { padding-bottom: 2.5rem; }
  .demo-hero {
    grid-template-columns: 1fr;
    gap: 2.2rem;
    padding-top: 2.3rem;
  }
  .demo-count strong { font-size: 5.2rem; }
  .demo-copy { grid-template-columns: 1fr; gap: 1.4rem; }
  .demo-copy ul { grid-template-columns: 1fr; }
  .demo-actions {
    grid-column: auto;
    grid-template-columns: 1fr 1fr;
  }
}
@media (max-width: 430px) {
  .demo-topline,
  .demo-item-head { font-size: .72rem; }
  .demo-hero h1 { font-size: 2.2rem; }
  .demo-actions { grid-template-columns: 1fr; }
}
</style>

<div class="demo-shell">
  <header class="demo-intro">
    <div class="demo-topline">
      <div>
        <span class="demo-label">Project demos</span>
        <span class="demo-kicker">Selected work · 中文讲解</span>
      </div>
      <a class="demo-back" href="/cv/">CV / Resume ↗</a>
    </div>
    <div class="demo-hero">
      <div class="demo-count">
        <strong>02</strong>
        <span>PROJECTS</span>
      </div>
      <div>
        <h1>两个项目，<br>两条完整工作流</h1>
        <p>从真实操作流程与运行结果开始，再进入仓库检查实现、测试和评测证据。</p>
      </div>
    </div>
  </header>

  <section class="demo-item" id="code-agent">
    <header class="demo-item-head">
      <span><strong>01 / 02</strong>&nbsp;&nbsp; Code Agent</span>
      <span>11:05</span>
    </header>
    <div class="demo-player">
      <video controls preload="metadata" playsinline poster="/images/demos/code-agent-v34.jpg">
        <source src="/assets/videos/code-agent-demo-v34-zh.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="demo-copy">
      <div>
        <h2>本地编码智能体</h2>
        <p class="demo-subtitle">从最小 Agent 循环到可恢复、可审查的仓库级交付。</p>
      </div>
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
    <header class="demo-item-head">
      <span><strong>02 / 02</strong>&nbsp;&nbsp; Minibrain</span>
      <span>07:10</span>
    </header>
    <div class="demo-player">
      <video controls preload="metadata" playsinline poster="/images/demos/minibrain-v20.jpg">
        <source src="/assets/videos/minibrain-demo-v20-zh.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
      </video>
    </div>
    <div class="demo-copy">
      <div>
        <h2>企业知识库问答与 LLM Wiki</h2>
        <p class="demo-subtitle">让不同的数据进入正确的检索链路，并交付可验证答案。</p>
      </div>
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
