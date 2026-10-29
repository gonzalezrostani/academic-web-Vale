---
title: 
layout: docs  # Do not modify.
---

<style>
/* Website fonts are already loaded by the Academic theme. */
#vgr-toolkit{--tool-accent:#667eea;--tool-purple:#764ba2;--tool-ink:#1f2937;--tool-muted:#6b7280;--tool-line:#e5e7eb;max-width:1100px;margin:0 auto;font-family:'Roboto',sans-serif;font-size:inherit;line-height:1.65;color:var(--tool-ink);text-align:left}
#vgr-toolkit *,#vgr-toolkit *::before,#vgr-toolkit *::after{box-sizing:border-box}
#vgr-toolkit [hidden]{display:none!important}
#vgr-toolkit h1,#vgr-toolkit h2{font-family:'Montserrat',sans-serif;color:var(--tool-ink);letter-spacing:normal;text-transform:none}
#vgr-toolkit button{font-family:inherit}
#vgr-toolkit a:focus-visible,#vgr-toolkit button:focus-visible,#vgr-toolkit pre:focus-visible{outline:3px solid var(--tool-accent);outline-offset:4px}
/* Same gradient and rounded hero as the research and teaching pages. */
#vgr-toolkit .toolkit-hero{text-align:center;margin:0 0 26px;padding:28px 18px;background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);border-radius:18px;color:#fff}
#vgr-toolkit .toolkit-hero h1{font-size:2.1em;font-weight:700;line-height:1.25;margin:0 0 10px;color:#fff}
#vgr-toolkit .toolkit-hero p{font-size:1.05em;opacity:.95;max-width:980px;margin:0 auto;line-height:1.6;color:#fff}
/* Filters are shown only when JavaScript is available. */
#vgr-toolkit .tool-filters{background:#fafaff;border:1px solid var(--tool-line);border-radius:16px;padding:18px 20px;margin:0 0 22px}
#vgr-toolkit .tool-controls{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin:0 0 12px}
#vgr-toolkit .tool-controls .label{font-weight:700;color:var(--tool-ink)}
#vgr-toolkit .tool-pills{display:flex;gap:8px;flex-wrap:wrap}
#vgr-toolkit .tool-pill{padding:8px 14px;border-radius:999px;border:2px solid var(--tool-line);background:#fff;color:var(--tool-ink);cursor:pointer;font-weight:700;font-size:.9em;line-height:1.4;transition:background .2s ease,border-color .2s ease,color .2s ease;user-select:none}
#vgr-toolkit .tool-pill:hover{border-color:var(--tool-accent)}
#vgr-toolkit .tool-pill.active{background:var(--tool-accent);border-color:var(--tool-accent);color:#fff}
#vgr-toolkit .tool-count{font-size:.84em;color:var(--tool-muted);margin:0}
/* Cards keep their original frame, with the teaching page's blue accent. */
#vgr-toolkit .tool-card{min-width:0}
#vgr-toolkit .tool-box{background:#fff;border:1px solid var(--tool-line);border-left:6px solid #a7b7ff;border-radius:14px;padding:20px 22px;box-shadow:0 2px 10px rgba(0,0,0,.04);transition:box-shadow .2s ease,transform .2s ease;margin:0 0 20px}
#vgr-toolkit .tool-box:hover{box-shadow:0 8px 24px rgba(0,0,0,.08);transform:translateY(-1px)}
#vgr-toolkit .tool-title{margin:0 0 8px;font-weight:700;font-size:1.3em;line-height:1.4;overflow-wrap:break-word}
#vgr-toolkit .tool-title em{font-style:italic}
#vgr-toolkit .tool-meta{color:var(--tool-muted);font-size:.98em;margin:0 0 12px}
#vgr-toolkit .tool-body{color:#374151;line-height:1.65}
#vgr-toolkit .tool-body p{margin:0 0 12px}
#vgr-toolkit .tool-body>div+p{margin-top:10px}
/* Buttons remain beside one another; narrow screens can scroll the row. */
#vgr-toolkit .tool-actions{display:flex;flex-wrap:nowrap;gap:10px;margin:12px 0 0;overflow-x:auto;-webkit-overflow-scrolling:touch;padding:3px 2px 6px;scrollbar-width:thin}
#vgr-toolkit .tool-actions::-webkit-scrollbar{height:6px}
#vgr-toolkit .tool-actions::-webkit-scrollbar-thumb{background:var(--tool-line);border-radius:999px}
#vgr-toolkit .action-btn{display:inline-flex;align-items:center;justify-content:center;padding:8px 12px;border-radius:8px;border:1px solid #b21619;color:#b21619;text-decoration:none!important;font-family:inherit;font-weight:700;font-size:.9em;line-height:1.5;transition:background .2s ease,color .2s ease;background:#fff;white-space:nowrap;flex:0 0 auto}
#vgr-toolkit .action-btn:hover{background:#b21619;color:#fff}
#vgr-toolkit .action-btn.blue{border-color:#3b82f6;color:#2563eb}
#vgr-toolkit .action-btn.blue:hover{background:#3b82f6;color:#fff}
#vgr-toolkit .action-btn.gray{border-color:#6b7280;color:#374151}
#vgr-toolkit .action-btn.gray:hover{background:#374151;color:#fff}
#vgr-toolkit .tool-tags{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px}
#vgr-toolkit .tool-tag{padding:4px 10px;border-radius:999px;background:#f3f4f6;border:1px solid var(--tool-line);color:#111827;font-weight:700;font-size:.78em}
/* Keep installation code readable without widening the page. */
#vgr-toolkit pre{font-family:'Roboto Mono',monospace;font-size:.85em;line-height:1.6;max-width:100%;overflow-x:auto;white-space:pre;background:#f8fafc;border:1px solid var(--tool-line);border-radius:10px;padding:14px 16px;margin:12px 0 0;color:#374151;tab-size:2}
#vgr-toolkit pre code{display:block;font-family:inherit;font-size:inherit;line-height:inherit;white-space:inherit;background:transparent;color:inherit;padding:0;border:0}
@media(max-width:700px){#vgr-toolkit .toolkit-hero h1{font-size:1.85em}#vgr-toolkit .toolkit-hero{padding:26px 18px}#vgr-toolkit .tool-filters{padding:16px}#vgr-toolkit .tool-controls{align-items:flex-start}#vgr-toolkit .tool-controls .label{width:100%}#vgr-toolkit .tool-box{padding:18px 16px}#vgr-toolkit .tool-title{font-size:1.15em}#vgr-toolkit .action-btn{font-size:.86em;padding:8px 10px}#vgr-toolkit .tool-box:hover{transform:none}}
@media(prefers-reduced-motion:reduce){#vgr-toolkit *{transition:none!important}#vgr-toolkit .tool-box:hover{transform:none}}
@media print{#vgr-toolkit .tool-filters{display:none!important}#vgr-toolkit .tool-card[hidden]{display:block!important}#vgr-toolkit .toolkit-hero{background:none;border:1px solid var(--tool-line);color:#000}#vgr-toolkit .toolkit-hero h1,#vgr-toolkit .toolkit-hero p{color:#000}#vgr-toolkit .tool-box{break-inside:avoid;box-shadow:none}}
</style>
<div id="vgr-toolkit">
<header class="toolkit-hero">
<h1>📚 Research Toolkit</h1>
<p>Tools, notes, and side projects I’ve put together over time—mostly beginner-friendly, designed as useful starting points for research workflows. I’ll keep updating this space as I systematize more of my work.</p>
</header>
<div class="tool-filters" hidden>
<div class="tool-controls">
<span class="label" id="tool-topic-label">Topic:</span>
<div class="tool-pills" role="group" aria-labelledby="tool-topic-label">
<button type="button" class="tool-pill active" data-topic="all" aria-pressed="true">All</button>
<button type="button" class="tool-pill" data-topic="methods" aria-pressed="false">📊 Methods</button>
<button type="button" class="tool-pill" data-topic="professionalization" aria-pressed="false">🎓 Professionalization</button>
<button type="button" class="tool-pill" data-topic="tools" aria-pressed="false">🧰 Tools</button>
</div>
</div>
<p class="tool-count" role="status" aria-live="polite" aria-atomic="true">Showing all 11 resources</p>
</div>
<section class="tool-resources" aria-label="Toolkit resources">
<article class="tool-card" aria-labelledby="tool-title-1" data-topics="methods tools">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-1">📊 R Package: <em>tscsdep</em></h2>
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
<a class="action-btn blue" href="https://github.com/judechays/STADL" target="_blank" rel="noopener noreferrer">🐙 GitHub</a>
</div>
<div class="tool-body" style="margin-top:12px">
<strong>Installation 📥</strong>
</div>
<pre tabindex="0" aria-label="R package installation code"><code class="language-r">library(devtools)
devtools::install_github("judechays/STADL", dependencies = TRUE)</code></pre>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-2" data-topics="methods tools">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-2">🤖 AI as a Research Tool</h2>
<div class="tool-meta">Failing faster, learning better in social science research</div>
<div class="tool-body">
<p>A slide handout covering six applications of AI: annotation and measurement, experiments, synthetic surveys, simulations, data collection, and AI auditing. Includes examples and best practices for testing ideas, detecting failures early, and validating results.</p>
<div class="tool-tags">
<span class="tool-tag">AI</span>
<span class="tool-tag">Research Methods</span>
<span class="tool-tag">Social Science</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/ai_social_science_research_en_v22_handout.pdf" target="_blank" rel="noopener noreferrer" hreflang="en">📄 English (PDF)</a>
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/ia_investigacion_ciencias_sociales_es_v21_handout.pdf" target="_blank" rel="noopener noreferrer" hreflang="es" lang="es">📄 Español (PDF)</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-3" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-3">📅 5-year PhD Plan  </h2>
<div class="tool-meta">Notes based on my experience—things I wish I had known before starting</div>
<div class="tool-body">
<p>Five years in a PhD can go by quickly, so it helps to have a plan from the start. I wrote this guide for students I advise and those considering working with me. It covers coursework, research, preparation for academic and industry jobs, and how we will work together.</p>
<div class="tool-tags">
<span class="tool-tag">Grad School</span>
<span class="tool-tag">Planning</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/5ys_PhD_Advising_Guidelines.pdf" target="_blank" rel="noopener noreferrer">📄 Read the guide</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-3" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-3">🎓 Starting Your PhD</h2>
<div class="tool-meta">Notes based on my experience—things I wish I had known before starting</div>
<div class="tool-body">
<p>A set of notes focused on the summer and weeks leading up to the PhD, with practical advice on routines, expectations, and early decisions that matter.</p>
<div class="tool-tags">
<span class="tool-tag">Grad School</span>
<span class="tool-tag">Planning</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/StartingPhD2.pdf" target="_blank" rel="noopener noreferrer">📄 Read the guide</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-4" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-4">📢 Presentation Tips</h2>
<div class="tool-meta">How to structure research presentations effectively</div>
<div class="tool-body">
<p>Prepared for final paper presentations at the MPE Summer Methods Camp, with strategies for narrative flow, slide discipline, and delivery.</p>
<div class="tool-tags">
<span class="tool-tag">Slides</span>
<span class="tool-tag">Communication</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/presentation_mpe" target="_blank" rel="noopener noreferrer">📄 Download</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-5" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-5">💬 Discussant Guide</h2>
<div class="tool-meta">How to prepare constructive comments for conferences and workshops</div>
<div class="tool-body">
<p>A guide for graduate students on evaluating research, selecting consequential comments, preparing discussant slides, offering practical suggestions, and encouraging a productive scholarly discussion.</p>
<div class="tool-tags">
<span class="tool-tag">Conferences</span>
<span class="tool-tag">Professionalization</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/discussant.pdf" target="_blank" rel="noopener noreferrer">📄 Download</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-6" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-6">🎤 Job Talk Tips</h2>
<div class="tool-meta">Notes on how to structure and deliver a strong job talk</div>
<div class="tool-body">
<p>A collection of notes based on feedback I’ve received and observed from others. Disclaimer: not a definitive guide—just consolidated lessons that tend to help.</p>
<div class="tool-tags">
<span class="tool-tag">Job Market</span>
<span class="tool-tag">Talks</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/How_to_give_jobtalk.pdf" target="_blank" rel="noopener noreferrer">📄 Read the guide</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-7" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-7">☕ Visiting Scholar Meetings</h2>
<div class="tool-meta">Preparing for one-on-one meetings and breakfasts</div>
<div class="tool-body">
<p>A guide for graduate students on what to expect from meetings with visiting scholars, preparing a concise elevator pitch, discussing research ideas, seeking feedback, and learning about academic life. Includes sample pitches and questions to help the conversation flow.</p>
<div class="tool-tags">
<span class="tool-tag">Visiting Scholars</span>
<span class="tool-tag">Professionalization</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/papers/Visiting.pdf" target="_blank" rel="noopener noreferrer">📄 Download</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-8" data-topics="tools">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-8">📝 LaTeX Tips</h2>
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
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Latex-Tips" target="_blank" rel="noopener noreferrer">🐙 GitHub</a>
<a class="action-btn" href="https://www.overleaf.com/read/rrdfvjbpfyrq" target="_blank" rel="noopener noreferrer">📄 Overleaf</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-9" data-topics="tools professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-9">🐙 Getting Started with GitHub</h2>
<div class="tool-meta">A beginner-friendly guide to using Git and GitHub effectively</div>
<div class="tool-body">
<p>Notes and examples to help you build a simple workflow: clone, commit, push, branches, and common troubleshooting.</p>
<div class="tool-tags">
<span class="tool-tag">Git</span>
<span class="tool-tag">Workflow</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Beginning-with-Git/blob/master/labNotes.md" target="_blank" rel="noopener noreferrer">🐙 GitHub</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-10" data-topics="methods tools">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-10">🤖 Introduction to SVM & Scikit-Learn</h2>
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
<a class="action-btn blue" href="https://github.com/gonzalezrostani/Support-Vector-Machine" target="_blank" rel="noopener noreferrer">🐙 GitHub</a>
<a class="action-btn" href="https://pitt.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5f994000-d1d1-49bf-bec2-ac810157b3b6" target="_blank" rel="noopener noreferrer">🎥 Tutorial Video</a>
</div>
</div>
</article>
<article class="tool-card" aria-labelledby="tool-title-11" data-topics="professionalization">
<div class="tool-box">
<h2 class="tool-title" id="tool-title-11">🔍 Data Access & Research Transparency in Political Science</h2>
<div class="tool-meta">Professionalization guide on transparency and accessibility</div>
<div class="tool-body">
<p>A short guide focused on concrete steps for ensuring transparency, reproducibility, and data accessibility in political science research.</p>
<div class="tool-tags">
<span class="tool-tag">Transparency</span>
<span class="tool-tag">Replication</span>
</div>
</div>
<div class="tool-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/Professionalization.pdf" target="_blank" rel="noopener noreferrer">📄 Read the document</a>
</div>
</div>
</article>
</section>
</div>
<script>
(function () {
  var root = document.getElementById('vgr-toolkit');
  if (!root || root.dataset.ready === 'true') return;
  root.dataset.ready = 'true';
  var buttons = Array.from(root.querySelectorAll('.tool-pill'));
  var cards = Array.from(root.querySelectorAll('.tool-card'));
  var count = root.querySelector('.tool-count');
  root.querySelector('.tool-filters').hidden = false;
  buttons.forEach(function (button) {
    button.addEventListener('click', function () {
      var topic = button.dataset.topic;
      buttons.forEach(function (item) {
        var selected = item === button;
        item.classList.toggle('active', selected);
        item.setAttribute('aria-pressed', String(selected));
      });
      var visible = 0;
      cards.forEach(function (card) {
        var topics = (card.dataset.topics || '').split(' ');
        var show = topic === 'all' || topics.includes(topic);
        card.hidden = !show;
        if (show) visible++;
      });
      count.textContent = visible === cards.length
        ? 'Showing all ' + cards.length + ' resources'
        : 'Showing ' + visible + ' of ' + cards.length + ' resources';
    });
  });
})();
</script>
