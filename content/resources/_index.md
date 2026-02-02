---
title: 
layout: docs  # Do not modify.
---

<style>
/* HERO BOX (Toolkit) */
.toolkit-hero{
text-align:center;
margin:0 0 26px;
padding:28px 18px;
background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);
border-radius:18px;
color:#fff
}
.toolkit-hero h1{
font-family:inherit;
font-size:2.1em;
font-weight:800;
margin:0 0 10px
}
.toolkit-hero p{
font-size:1.05em;
opacity:.95;
max-width:980px;
margin:0 auto;
line-height:1.6
}

/* FILTER BAR (Topics) */
.tool-controls{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin:14px 0 18px}
.tool-controls .label{font-weight:800;color:#1f2937}
.tool-pills{display:flex;gap:10px;flex-wrap:wrap}
.tool-pill{padding:8px 14px;border-radius:999px;border:2px solid #e5e7eb;background:#fff;cursor:pointer;font-weight:800;font-size:.92em;transition:all .2s ease;user-select:none}
.tool-pill:hover{border-color:#667eea}
.tool-pill.active{background:#667eea;border-color:#667eea;color:#fff}
.tool-card.hidden{display:none}

/* TOOL CARD (boxes) */
.tool-box{
background:#fff;
border:1px solid #e5e7eb;
border-radius:14px;
padding:18px;
box-shadow:0 2px 10px rgba(0,0,0,.04);
transition:all .2s ease;
margin:12px 0 18px
}
.tool-box:hover{
box-shadow:0 8px 24px rgba(0,0,0,.08);
transform:translateY(-1px)
}
.tool-title{margin:0 0 6px;font-weight:900}
.tool-meta{color:#6b7280;font-size:.98em;margin:0 0 12px}
.tool-body{color:#374151;line-height:1.65}

/* BUTTONS (like research page) */
.tool-actions{
display:flex;
flex-wrap:nowrap;
gap:10px;
margin:10px 0 0;
overflow-x:auto;
-webkit-overflow-scrolling:touch;
padding-bottom:2px;
}
.tool-actions::-webkit-scrollbar{height:6px}
.tool-actions::-webkit-scrollbar-thumb{background:#e5e7eb;border-radius:999px}
@media (min-width: 700px){
.tool-actions{overflow-x:visible}
}
.action-btn{
display:inline-block;
padding:8px 12px;
border-radius:8px;
border:1px solid #b21619;
color:#b21619;
text-decoration:none !important;
font-weight:900;
font-size:.9em;
transition:all .2s ease;
background:#fff;
white-space:nowrap;
flex:0 0 auto;
}
.action-btn:hover{background:#b21619;color:#fff}
.action-btn.blue{border-color:#3b82f6;color:#2563eb}
.action-btn.blue:hover{background:#3b82f6;color:#fff}
.action-btn.gray{border-color:#6b7280;color:#374151}
.action-btn.gray:hover{background:#374151;color:#fff}

/* Small tag row inside cards (optional) */
.tool-tags{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px}
.tool-tag{padding:4px 10px;border-radius:999px;background:#f3f4f6;border:1px solid #e5e7eb;color:#111827;font-weight:800;font-size:.78em}
</style>

<div class="toolkit-hero">
<h1>📚 Research Toolkit</h1>
<p>Tools, notes, and side projects I’ve put together over time—mostly beginner-friendly, designed as useful starting points for research workflows. I’ll keep updating this space as I systematize more of my work.</p>
</div>

<div class="tool-controls">
<span class="label">Topic:</span>
<div class="tool-pills">
<button class="tool-pill active" data-kind="topic" onclick="setToolTopic('all', this)">All</button>
<button class="tool-pill" data-kind="topic" onclick="setToolTopic('methods', this)">📊 Methods</button>
<button class="tool-pill" data-kind="topic" onclick="setToolTopic('professionalization', this)">🎓 Professionalization</button>
<button class="tool-pill" data-kind="topic" onclick="setToolTopic('tools', this)">🧰 Tools</button>
</div>
</div>

<script>
let toolTopic='all';

function setActive(kind, el){
document.querySelectorAll('.tool-pill[data-kind="'+kind+'"]').forEach(b=>b.classList.remove('active'));
if(el) el.classList.add('active');
}

function setToolTopic(topic, el){
toolTopic=topic;
setActive('topic', el);
applyToolFilters();
}

function applyToolFilters(){
document.querySelectorAll('.tool-card').forEach(card=>{
const topics=(card.dataset.topics || '').split(' ').filter(Boolean);
const okTopic=(toolTopic==='all') || (topics.includes(toolTopic));
card.classList.toggle('hidden', !okTopic);
});
}
</script>

<!-- tscsdep -->
<article class="tool-card" data-topics="methods tools">
<div class="tool-box">
<h3 class="tool-title">📊 R Package: <em>tscsdep</em></h3>
<div class="tool-meta">Tools for analyzing country-year TSCS data with spatial and temporal dependence</div>

<div class="tool-body">
<div><strong>Authors:</strong> Hays, Jude C., Valentina González-Rostani, Scott Cook, Robert Franzese, and Wooseok Kim (2022). Version 0.1.0.</div>
<p>This package provides functions for creating geographic spatial weights matrices and estimating spatial models. It supports unbalanced data up to 2019 and includes wrappers for SAR, SEM, and SAC models.</p>

<div class="tool-tags">
<span class="tool-tag">Spatial</span>
<span class="tool-tag">TSCS</span>
<span class="tool-tag">R</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn blue" href="https://github.com/judechays/STADL" target="_blank" rel="noopener">🐙 GitHub</a>
</div>

<div class="tool-body" style="margin-top:12px">
<strong>Installation 📥</strong>
</div>

<pre><code class="language-r">library(devtools)
devtools::install_github("judechays/STADL", dependencies = TRUE)</code></pre>
</div>
</article>

<!-- Starting your PhD -->
<article class="tool-card" data-topics="professionalization">
<div class="tool-box">
<h3 class="tool-title">🎓 Starting Your PhD</h3>
<div class="tool-meta">Notes based on my experience—things I wish I had known before starting</div>

<div class="tool-body">
<p>A set of notes focused on the summer and weeks leading up to the PhD, with practical advice on routines, expectations, and early decisions that matter.</p>

<div class="tool-tags">
<span class="tool-tag">Grad School</span>
<span class="tool-tag">Planning</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/StartingPhD2.pdf" target="_blank" rel="noopener">📄 Read the guide</a>
</div>
</div>
</article>

<!-- Presentation Tips -->
<article class="tool-card" data-topics="professionalization">
<div class="tool-box">
<h3 class="tool-title">📢 Presentation Tips</h3>
<div class="tool-meta">How to structure research presentations effectively</div>

<div class="tool-body">
<p>Prepared for final paper presentations at the MPE Summer Methods Camp, with strategies for narrative flow, slide discipline, and delivery.</p>

<div class="tool-tags">
<span class="tool-tag">Slides</span>
<span class="tool-tag">Communication</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/presentation_mpe" target="_blank" rel="noopener">📄 Download</a>
</div>
</div>
</article>

<!-- Job Talk Tips -->
<article class="tool-card" data-topics="professionalization">
<div class="tool-box">
<h3 class="tool-title">🎤 Job Talk Tips</h3>
<div class="tool-meta">Notes on how to structure and deliver a strong job talk</div>

<div class="tool-body">
<p>A collection of notes based on feedback I’ve received and observed from others. Disclaimer: not a definitive guide—just consolidated lessons that tend to help.</p>

<div class="tool-tags">
<span class="tool-tag">Job Market</span>
<span class="tool-tag">Talks</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/How_to_give_jobtalk.pdf" target="_blank" rel="noopener">📄 Read the guide</a>
</div>
</div>
</article>

<!-- LaTeX Tips -->
<article class="tool-card" data-topics="tools">
<div class="tool-box">
<h3 class="tool-title">📝 LaTeX Tips</h3>
<div class="tool-meta">Useful LaTeX tips and tricks to streamline your workflow</div>

<div class="tool-body">
<p>A collection of snippets and small patterns I reuse frequently (tables, figures, Beamer, macros, and workflow conveniences).</p>

<div class="tool-tags">
<span class="tool-tag">LaTeX</span>
<span class="tool-tag">Overleaf</span>
<span class="tool-tag">Writing</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Latex-Tips" target="_blank" rel="noopener">🐙 GitHub</a>
<a class="action-btn" href="https://www.overleaf.com/read/rrdfvjbpfyrq" target="_blank" rel="noopener">📄 Overleaf</a>
</div>
</div>
</article>

<!-- Getting Started with GitHub -->
<article class="tool-card" data-topics="tools professionalization">
<div class="tool-box">
<h3 class="tool-title">🐙 Getting Started with GitHub</h3>
<div class="tool-meta">A beginner-friendly guide to using Git and GitHub effectively</div>

<div class="tool-body">
<p>Notes and examples to help you build a simple workflow: clone, commit, push, branches, and common troubleshooting.</p>

<div class="tool-tags">
<span class="tool-tag">Git</span>
<span class="tool-tag">Workflow</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Beginning-with-Git/blob/master/labNotes.md" target="_blank" rel="noopener">🐙 GitHub</a>
</div>
</div>
</article>

<!-- SVM & Scikit-Learn -->
<article class="tool-card" data-topics="methods tools">
<div class="tool-box">
<h3 class="tool-title">🤖 Introduction to SVM & Scikit-Learn</h3>
<div class="tool-meta">Support Vector Machines (SVM) and how to implement them in scikit-learn</div>

<div class="tool-body">
<p>An accessible walkthrough of the intuition behind SVMs, plus implementation examples and a tutorial video.</p>

<div class="tool-tags">
<span class="tool-tag">ML</span>
<span class="tool-tag">Python</span>
<span class="tool-tag">SVM</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Support-Vector-Machine" target="_blank" rel="noopener">🐙 GitHub</a>
<a class="action-btn" href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5f994000-d1d1-49bf-bec2-ac810157b3b6" target="_blank" rel="noopener">🎥 Tutorial Video</a>
</div>
</div>
</article>

<!-- Transparency -->
<article class="tool-card" data-topics="professionalization">
<div class="tool-box">
<h3 class="tool-title">🔍 Data Access & Research Transparency in Political Science</h3>
<div class="tool-meta">Professionalization guide on transparency and accessibility</div>

<div class="tool-body">
<p>A short guide focused on concrete steps for ensuring transparency, reproducibility, and data accessibility in political science research.</p>

<div class="tool-tags">
<span class="tool-tag">Transparency</span>
<span class="tool-tag">Replication</span>
</div>
</div>

<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/Professionalization.pdf" target="_blank" rel="noopener">📄 Read the document</a>
</div>
</div>
</article>
