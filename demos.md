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
.masthead__inner-wrap,
.greedy-nav,
.page__footer {
  background: #f7f7f3;
}
.masthead { border-bottom: 1px solid #d9dadd; }
.page__title { display: none; }
.page {
  float: none !important;
  width: 100% !important;
  padding-right: 0 !important;
}
.page__inner-wrap {
  max-width: 1120px;
  margin: 0 auto;
}
.page__content { margin-top: 0; }
.demo-shell {
  --ink: #101113;
  --muted: #73757a;
  --rule: #d9dadd;
  --blue: #315cf5;
  max-width: 1120px;
  margin: 0 auto;
  color: var(--ink);
  font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Hiragino Sans GB", sans-serif;
}
.demo-intro {
  display: grid;
  grid-template-columns: minmax(0, 1fr) auto;
  gap: 2rem;
  align-items: end;
  padding: 2.1rem 0 1.55rem;
  border-bottom: 1px solid var(--rule);
}
.demo-kicker {
  color: var(--blue);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  font-weight: 600;
  letter-spacing: .08em;
  text-transform: uppercase;
}
.demo-intro h1 {
  margin: .48rem 0 0;
  color: var(--ink);
  font-size: clamp(2rem, 4vw, 3.2rem);
  font-weight: 650;
  line-height: 1.12;
  letter-spacing: -.035em;
}
.demo-intro p {
  max-width: 650px;
  margin: .72rem 0 0;
  color: var(--muted);
  font-size: 1rem;
  line-height: 1.7;
}
.demo-back {
  padding-bottom: .25rem;
  border-bottom: 1px solid var(--blue);
  color: var(--ink) !important;
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  font-weight: 600;
  letter-spacing: .025em;
  text-decoration: none !important;
  white-space: nowrap;
}
.demo-item {
  display: grid;
  grid-template-columns: minmax(0, 1.58fr) minmax(280px, .82fr);
  gap: 1.4rem 2.3rem;
  padding: 1.65rem 0 2.6rem;
  border-bottom: 1px solid var(--rule);
  scroll-margin-top: 2rem;
}
.demo-item-head {
  grid-column: 1 / -1;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1.5rem;
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  letter-spacing: .055em;
  text-transform: uppercase;
}
.demo-item-head strong {
  color: var(--blue);
  font-weight: 600;
}
.demo-item-head span:last-child { color: var(--muted); }
.demo-player {
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border: 1px solid var(--rule);
  border-radius: 2px;
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
  align-self: center;
}
.demo-copy h2 {
  margin: 0;
  color: var(--ink);
  font-size: clamp(1.45rem, 2.4vw, 1.8rem);
  font-weight: 650;
  line-height: 1.3;
  letter-spacing: -.025em;
}
.demo-subtitle {
  margin: .55rem 0 1.1rem;
  color: var(--muted);
  font-size: .95rem;
  line-height: 1.65;
}
.demo-copy ul {
  margin: 0 0 1.15rem;
  padding: 0;
  list-style: none;
}
.demo-copy li {
  position: relative;
  margin: 0;
  padding: .48rem 0 .48rem 1rem;
  border-top: 1px solid var(--rule);
  color: #393a3d;
  font-size: .9rem;
  line-height: 1.5;
}
.demo-copy li::before {
  position: absolute;
  top: 1.08rem;
  left: 0;
  width: 5px;
  height: 2px;
  background: var(--blue);
  content: "";
}
.demo-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1.25rem;
}
.demo-button {
  padding-bottom: .2rem;
  border-bottom: 1px solid var(--rule);
  color: var(--ink) !important;
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .76rem;
  font-weight: 600;
  text-decoration: none !important;
}
.demo-button::after {
  margin-left: .35rem;
  color: var(--blue);
  content: "↗";
}
.demo-button.primary {
  border-bottom-color: var(--blue);
  color: var(--blue) !important;
}
.demo-note {
  margin: 1rem 0 0;
  color: var(--muted);
  font-size: .8rem;
  line-height: 1.6;
}
.demo-back:hover,
.demo-button:hover { color: var(--blue) !important; }
.demo-back:focus-visible,
.demo-button:focus-visible,
.demo-player video:focus-visible {
  outline: 2px solid var(--blue);
  outline-offset: 4px;
}
@media (max-width: 820px) {
  .demo-intro { padding-top: 1.6rem; }
  .demo-item {
    grid-template-columns: 1fr;
    gap: 1rem;
    padding-top: 1.35rem;
  }
  .demo-item-head { grid-column: auto; }
  .demo-copy { padding-top: .45rem; }
  .demo-copy ul {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0 1.25rem;
  }
}
@media (max-width: 520px) {
  .demo-intro {
    grid-template-columns: 1fr;
    gap: 1rem;
  }
  .demo-intro h1 { font-size: 2rem; }
  .demo-copy ul { grid-template-columns: 1fr; }
}
</style>

<div class="demo-shell">
  <header class="demo-intro">
    <div>
      <div class="demo-kicker">Project demos · 02 projects</div>
      <h1>项目视频演示</h1>
      <p>Code Agent 与 Minibrain 的完整工作流、实现重点和评测结果。</p>
    </div>
    <a class="demo-back" href="/cv/">CV / Resume ↗</a>
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
