---
title: "Project Demos"
permalink: /demos/
layout: single
author_profile: false
classes: wide
---

<style>
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
.page__content { margin-top: .8rem; }
.demo-shell {
  --ink: #101828;
  --muted: #5f6876;
  --line: #dce2ec;
  --accent: #2859d9;
  --accent-soft: #edf2ff;
  --surface: #ffffff;
  max-width: 1160px;
  margin: 0 auto;
  color: var(--ink);
}
.demo-intro {
  position: relative;
  display: grid;
  grid-template-columns: minmax(0, 1fr) auto;
  align-items: end;
  gap: 1.5rem;
  overflow: hidden;
  padding: clamp(1.5rem, 4vw, 2.7rem);
  border: 1px solid #d8e0ee;
  border-radius: 22px;
  background:
    radial-gradient(circle at 88% 12%, rgba(40, 89, 217, .13), transparent 33%),
    linear-gradient(135deg, #ffffff 0%, #f5f7fc 100%);
  box-shadow: 0 16px 46px rgba(31, 45, 76, .08);
}
.demo-intro::before {
  position: absolute;
  inset: 0 auto 0 0;
  width: 4px;
  background: var(--accent);
  content: "";
}
.demo-kicker {
  margin-bottom: .65rem;
  color: var(--accent);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .78rem;
  font-weight: 800;
  letter-spacing: .11em;
  text-transform: uppercase;
}
.demo-intro h1 {
  margin: 0;
  color: var(--ink);
  font-size: clamp(2.35rem, 5vw, 4.25rem);
  line-height: 1;
  letter-spacing: -.045em;
}
.demo-intro p {
  max-width: 680px;
  margin: 1rem 0 0;
  color: var(--muted);
  font-size: 1.02rem;
  line-height: 1.75;
}
.demo-back {
  display: inline-flex;
  align-items: center;
  min-height: 2.55rem;
  padding: .58rem .95rem;
  border: 1px solid #cdd6e5;
  border-radius: 999px;
  background: rgba(255, 255, 255, .78);
  color: var(--ink) !important;
  white-space: nowrap;
  font-size: .88rem;
  font-weight: 750;
  text-decoration: none !important;
  box-shadow: 0 4px 14px rgba(31, 45, 76, .06);
}
.demo-item {
  display: grid;
  grid-template-columns: minmax(0, 1.55fr) minmax(280px, .8fr);
  gap: clamp(1.5rem, 3vw, 2.25rem);
  align-items: center;
  margin-top: 1.35rem;
  padding: clamp(1rem, 2.5vw, 1.55rem);
  border: 1px solid var(--line);
  border-radius: 20px;
  background: var(--surface);
  box-shadow: 0 12px 34px rgba(31, 45, 76, .065);
  scroll-margin-top: 2rem;
}
.demo-player {
  overflow: hidden;
  aspect-ratio: 16 / 9;
  border: 1px solid #cfd7e3;
  border-radius: 14px;
  background: #090d16;
  box-shadow: 0 16px 34px rgba(16, 24, 40, .16);
}
.demo-player video {
  display: block;
  width: 100%;
  height: 100% !important;
  object-fit: cover;
  background: #090d16;
}
.demo-index {
  display: inline-flex;
  align-items: center;
  min-height: 1.85rem;
  padding: .28rem .58rem;
  border: 1px solid #d9e2f6;
  border-radius: 999px;
  background: var(--accent-soft);
  color: var(--accent);
  font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
  font-size: .75rem;
  font-weight: 700;
  letter-spacing: .055em;
}
.demo-copy h2 {
  margin: .72rem 0 .38rem;
  color: var(--ink);
  font-size: clamp(1.45rem, 2.4vw, 1.82rem);
  line-height: 1.25;
  letter-spacing: -.025em;
}
.demo-subtitle {
  margin: 0;
  color: var(--muted);
  font-size: .96rem;
  line-height: 1.65;
}
.demo-copy ul {
  margin: 1.05rem 0 1.3rem;
  padding: 0;
  list-style: none;
}
.demo-copy li {
  position: relative;
  margin-bottom: .52rem;
  padding-left: 1.05rem;
  color: #344054;
  font-size: .93rem;
  line-height: 1.55;
}
.demo-copy li::before {
  position: absolute;
  top: .66em;
  left: 0;
  width: 5px;
  height: 5px;
  border-radius: 50%;
  background: var(--accent);
  content: "";
}
.demo-actions {
  display: flex;
  flex-wrap: wrap;
  gap: .62rem;
}
.demo-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 2.55rem;
  padding: .58rem .92rem;
  border: 1px solid #cbd4e1;
  border-radius: 999px;
  color: var(--ink) !important;
  font-size: .86rem;
  font-weight: 750;
  text-decoration: none !important;
}
.demo-button.primary {
  border-color: var(--accent);
  background: var(--accent);
  color: white !important;
  box-shadow: 0 7px 18px rgba(40, 89, 217, .2);
}
.demo-note {
  margin: 1.15rem 0 .4rem;
  text-align: center;
  color: var(--muted);
  font-size: .82rem;
}
@media (prefers-reduced-motion: no-preference) {
  .demo-back,
  .demo-button,
  .demo-item { transition: transform .18s ease, box-shadow .18s ease, border-color .18s ease; }
  .demo-back:hover,
  .demo-button:hover { transform: translateY(-1px); }
  .demo-item:hover {
    border-color: #cbd6e8;
    box-shadow: 0 18px 44px rgba(31, 45, 76, .09);
  }
}
.demo-back:focus-visible,
.demo-button:focus-visible,
.demo-player video:focus-visible {
  outline: 3px solid rgba(40, 89, 217, .35);
  outline-offset: 3px;
}
@media (max-width: 820px) {
  .demo-intro,
  .demo-item { grid-template-columns: 1fr; }
  .demo-back { justify-self: start; }
  .demo-item { align-items: start; }
}
@media (max-width: 520px) {
  .page__content { margin-top: .35rem; }
  .demo-intro { border-radius: 17px; }
  .demo-item {
    margin-top: 1rem;
    padding: .78rem;
    border-radius: 17px;
  }
  .demo-player { border-radius: 11px; }
  .demo-copy { padding: .2rem .25rem .5rem; }
  .demo-actions { display: grid; grid-template-columns: 1fr 1fr; }
}
</style>

<div class="demo-shell">
  <header class="demo-intro">
    <div>
      <div class="demo-kicker">Selected work · 中文讲解</div>
      <h1>Project demos</h1>
      <p>两个完整项目演示：先看真实工作流与结果，再进入仓库检查实现、测试和评测证据。</p>
    </div>
    <a class="demo-back" href="/cv/">View CV →</a>
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
