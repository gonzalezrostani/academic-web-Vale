+++
widget = "blank"
headless = true
active = true
weight = 26
title = ""
subtitle = ""

[design]
  columns = "1"

[design.spacing]
  padding = ["40px", "0", "40px", "0"]
+++

<style>
@import url('https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600;700&family=Work+Sans:wght@400;500;600&display=swap');
/* Match the original research-page palette, fonts, and frame. */
#vgr-research{--vgr-ink:#1f2937;--vgr-muted:#6b7280;--vgr-accent:#667eea;--vgr-purple:#764ba2;--vgr-red:#b21619;--vgr-line:#e5e7eb;--vgr-soft:#f3f4f6;max-width:1100px;margin:0 auto;color:var(--vgr-ink);font-family:'Work Sans',sans-serif;font-size:inherit;line-height:1.6;text-align:left}
#vgr-research *{box-sizing:border-box}
#vgr-research [hidden]{display:none!important}
#vgr-research a{color:var(--vgr-purple);text-decoration:underline;text-underline-offset:3px;overflow-wrap:anywhere}
#vgr-research a:hover{color:var(--vgr-accent)}
#vgr-research :is(a,button,input,select,summary):focus-visible{outline:3px solid var(--vgr-accent);outline-offset:4px}
#vgr-research :is(h1,h2,h3,h4){font-family:'Crimson Pro',Georgia,serif;font-weight:700;color:var(--vgr-ink);line-height:1.3;letter-spacing:normal;text-transform:none}
#vgr-research h1{font-size:2.3em;margin:0 0 10px}
#vgr-research h2{font-size:1.9em;margin:34px 0 18px;border-bottom:3px solid var(--vgr-accent);padding-bottom:8px;display:inline-block}
#vgr-research h3{font-size:1.6em;margin:0 0 12px}
#vgr-research p{margin:0 0 14px}
#vgr-research .vgr-eyebrow{font-family:'Work Sans',sans-serif;font-size:.78em;font-weight:600;letter-spacing:.06em;text-transform:uppercase;color:var(--vgr-muted);margin:0 0 10px}
/* Original centered banner and rounded navigation controls. */
#vgr-research .vgr-header{text-align:center;padding:28px 18px;margin-bottom:28px;background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);border-radius:18px;color:#fff}
#vgr-research .vgr-header h1{color:#fff}
#vgr-research .vgr-intro{font-size:1.05em;opacity:.95;max-width:900px;margin:0 auto;line-height:1.6}
#vgr-research .vgr-jump{display:flex;flex-wrap:wrap;gap:10px;margin:0 0 8px}
#vgr-research .vgr-jump a,#vgr-research .vgr-section-nav a{padding:8px 14px;border-radius:999px;border:2px solid var(--vgr-line);background:#fff;color:var(--vgr-ink);text-decoration:none;font-weight:700;font-size:.85em;transition:border-color .2s ease,color .2s ease}
#vgr-research .vgr-jump a:hover,#vgr-research .vgr-section-nav a:hover{border-color:var(--vgr-accent);color:var(--vgr-purple)}
/* New narrative sections use the original paper-card frame. */
#vgr-research .vgr-area{display:grid;grid-template-columns:1.15fr 1fr;gap:36px;background:#fff;border:1px solid var(--vgr-line);border-left:5px solid var(--vgr-accent);border-radius:14px;padding:24px;margin-bottom:18px;box-shadow:0 2px 10px rgba(0,0,0,.04)}
#vgr-research .vgr-area-text p{font-size:.95em;line-height:1.7;margin-bottom:0;color:#374151}
#vgr-research .vgr-area-papers{padding-top:4px}
#vgr-research .vgr-examples{list-style:none;margin:0;padding:0}
#vgr-research .vgr-examples li{font-family:'Crimson Pro',Georgia,serif;font-size:1.13em;font-weight:600;line-height:1.4;margin:0 0 11px;padding:0 0 11px;border-bottom:1px solid var(--vgr-line)}
#vgr-research .vgr-examples li:last-child{border:0;margin-bottom:0;padding-bottom:0}
#vgr-research .vgr-examples a{color:#111827;text-decoration:none}
#vgr-research .vgr-examples a:hover{color:var(--vgr-accent);text-decoration:underline}
#vgr-research #research-publications{margin-top:34px}
#vgr-research .vgr-index-heading{display:flex;justify-content:space-between;gap:24px;align-items:end}
#vgr-research .vgr-index-heading h2{margin-top:0}
#vgr-research .vgr-text-link{color:var(--vgr-red);font-size:.85em;white-space:nowrap;margin-bottom:26px}
#vgr-research .vgr-index-note{font-size:.95em;color:var(--vgr-muted);max-width:850px}
#vgr-research .vgr-section-nav{display:flex;flex-wrap:wrap;gap:10px;margin:18px 0 24px}
#vgr-research .vgr-section-nav span{color:var(--vgr-muted);margin-left:4px;font-size:.9em}
#vgr-research .vgr-tools{background:#fff;border:1px solid var(--vgr-line);border-radius:14px;box-shadow:0 2px 10px rgba(0,0,0,.04);padding:18px;display:grid;grid-template-columns:1.2fr 1fr 1fr auto;gap:14px;align-items:end}
#vgr-research .vgr-tools label{display:block;font-weight:600;font-size:.8em;margin:0 0 6px;color:var(--vgr-ink)}
#vgr-research .vgr-tools :is(input,select,button){height:44px;background:#fff;border:2px solid var(--vgr-line);border-radius:8px;font:inherit;font-size:.8em;color:var(--vgr-ink);padding:8px 10px;width:100%;margin:0}
#vgr-research .vgr-tools :is(input,select):focus{border-color:var(--vgr-accent)}
#vgr-research .vgr-tools input{min-width:0}
#vgr-research .vgr-tools button{width:auto;cursor:pointer;border-radius:999px;padding:8px 15px;font-weight:600;color:#fff;background:var(--vgr-accent);border-color:var(--vgr-accent)}
#vgr-research .vgr-tools button:hover{background:var(--vgr-purple);border-color:var(--vgr-purple)}
#vgr-research #vgr-result-count{grid-column:1/-1;font-size:.8em;color:var(--vgr-muted);margin:0}
#vgr-research #vgr-no-results{padding:24px 0}
#vgr-research .vgr-paper-section{margin-top:34px}
#vgr-research h3.vgr-group-title{font-family:'Crimson Pro',Georgia,serif;font-size:1.6em;font-weight:700;padding:0 0 8px;border-bottom:3px solid var(--vgr-accent);margin:0 0 18px}
#vgr-research .vgr-group-title span{font-family:'Work Sans',sans-serif;font-size:.55em;font-weight:500;color:var(--vgr-muted);padding-left:8px}
/* Original publication cards, status colors, and topic pills. */
#vgr-research .vgr-paper{display:block;background:#fff;border:1px solid var(--vgr-line);border-left:5px solid var(--vgr-line);border-radius:14px;padding:18px;margin:0 0 18px;box-shadow:0 2px 10px rgba(0,0,0,.04);transition:border-color .2s ease,box-shadow .2s ease,transform .2s ease;scroll-margin-top:100px}
#vgr-research .vgr-paper:hover{border-left-color:var(--vgr-accent);box-shadow:0 8px 24px rgba(0,0,0,.08);transform:translateX(4px)}
#vgr-research .vgr-paper:target{border-left-color:var(--vgr-accent);outline:2px solid var(--vgr-accent);outline-offset:3px}
#vgr-research .vgr-paper-top{display:flex;justify-content:space-between;align-items:flex-start;gap:14px;margin-bottom:8px}
#vgr-research .vgr-paper h4{font-size:1.2em;font-weight:700;line-height:1.35;margin:0;color:#111827}
#vgr-research .vgr-paper h4 a{color:#111827;text-decoration:none}
#vgr-research .vgr-paper h4 a:hover{color:var(--vgr-accent)}
#vgr-research .vgr-badge{display:inline-block;flex-shrink:0;border-radius:999px;padding:6px 12px;font-size:.8em;font-weight:800;white-space:nowrap;line-height:1.45}
#vgr-research .vgr-badge-published{background:#c6f6d5;color:#22543d}
#vgr-research .vgr-badge-conditional,#vgr-research .vgr-badge-chapters{background:#bee3f8;color:#1e3a8a}
#vgr-research .vgr-badge-review{background:#feebc8;color:#7c2d12}
#vgr-research .vgr-badge-working,#vgr-research .vgr-badge-progress{background:#e5e7eb;color:#111827}
#vgr-research .vgr-authors{color:var(--vgr-muted);font-size:.9em;line-height:1.45;margin:0 0 6px}
#vgr-research .vgr-meta{color:var(--vgr-muted);font-size:.95em;line-height:1.45;margin:0 0 6px}
#vgr-research .vgr-book{color:var(--vgr-muted);font-size:.9em;margin:0 0 9px}
#vgr-research .vgr-tags{display:flex;flex-wrap:wrap;gap:8px;margin:10px 0 12px}
#vgr-research .vgr-tags span{padding:4px 10px;border-radius:999px;background:var(--vgr-soft);border:1px solid var(--vgr-line);color:#111827;font-weight:700;font-size:.78em}
#vgr-research .vgr-actions{display:flex;flex-wrap:wrap;align-items:center;gap:8px;margin:10px 0 0}
#vgr-research .vgr-actions :is(a,button){display:inline-flex;align-items:center;justify-content:center;padding:6px 10px;color:var(--vgr-red);background:#fff;border:1px solid var(--vgr-red);border-radius:8px;text-decoration:none;font-family:inherit;font-weight:800;font-size:.85em;line-height:1.6;white-space:nowrap;cursor:pointer;margin:0}
#vgr-research .vgr-actions :is(a,button):hover,#vgr-research .vgr-actions button[aria-expanded="true"]{color:#fff;background:var(--vgr-red)}
#vgr-research .vgr-recognition{font-size:.8em;margin:5px 0 12px}
/* Original red controls; abstracts retain valid, full-width disclosure panels. */
#vgr-research .vgr-abstract{display:block;margin:8px 0 0;max-width:100%}
#vgr-research .vgr-abstract.vgr-enhanced:not([open]){display:none}
#vgr-research .vgr-abstract summary{list-style:none;display:inline-block;margin:0;padding:6px 10px;color:var(--vgr-red);border:1px solid var(--vgr-red);border-radius:8px;cursor:pointer;font-weight:800;font-size:.85em;user-select:none}
#vgr-research .vgr-abstract summary::-webkit-details-marker{display:none}
#vgr-research .vgr-abstract summary:hover,#vgr-research .vgr-abstract[open] summary{color:#fff;background:var(--vgr-red)}
#vgr-research .vgr-abstract>div{margin-top:8px;padding:10px 12px;border:1px solid var(--vgr-line);border-radius:10px;background:#fff;box-shadow:0 1px 6px rgba(0,0,0,.06);max-width:100%}
#vgr-research .vgr-abstract p{font-size:.95em;color:#374151;line-height:1.6;margin:0 0 12px}
#vgr-research .vgr-abstract p:last-child{margin-bottom:0}
#vgr-research .vgr-abstract p.vgr-source{font-size:.8em}
#vgr-research #research-public-writing{margin-top:34px}
#vgr-research .vgr-public-writing{list-style:none;margin:0;padding:0}
#vgr-research .vgr-public-writing li{background:#fff;border:1px solid var(--vgr-line);border-left:5px solid var(--vgr-line);border-radius:14px;box-shadow:0 2px 10px rgba(0,0,0,.04);padding:18px;margin-bottom:18px;font-family:'Crimson Pro',Georgia,serif;font-size:1.2em;font-weight:700}
#vgr-research .vgr-public-writing li>a{color:#111827;text-decoration:none}
#vgr-research .vgr-public-writing li>a:hover{color:var(--vgr-accent)}
#vgr-research .vgr-public-writing span{display:block;font-family:'Work Sans',sans-serif;font-size:.75em;font-weight:400;color:var(--vgr-muted);margin-top:6px}
#vgr-research .vgr-footer{font-size:.85em;padding-top:22px;margin-top:22px;border-top:1px solid var(--vgr-line)}
#vgr-research :is(section,header){scroll-margin-top:85px}
@media(max-width:900px){#vgr-research .vgr-tools{grid-template-columns:1fr 1fr}#vgr-research .vgr-search{grid-column:1/-1}#vgr-research .vgr-tools button{justify-self:start}#vgr-research .vgr-area{gap:24px}}
@media(max-width:768px){#vgr-research .vgr-header h1{font-size:1.9em}#vgr-research .vgr-area{grid-template-columns:1fr;gap:22px;padding:18px}#vgr-research .vgr-area-papers{padding:0}#vgr-research .vgr-paper-top{flex-direction:column}#vgr-research .vgr-index-heading{display:block}#vgr-research .vgr-text-link{display:inline-block;margin:0 0 14px}#vgr-research .vgr-paper:hover{transform:none}}
@media(max-width:480px){#vgr-research .vgr-tools{grid-template-columns:1fr;padding:15px}#vgr-research .vgr-paper{padding:16px}#vgr-research .vgr-badge{white-space:normal}#vgr-research .vgr-jump a,#vgr-research .vgr-section-nav a{font-size:.8em;padding:7px 11px}}
@media(prefers-reduced-motion:reduce){#vgr-research .vgr-paper{transition:none}#vgr-research .vgr-paper:hover{transform:none}}
@media print{#vgr-research{max-width:none;font-size:10pt;color:#000}#vgr-research .vgr-header{background:none;color:#000;border:1px solid var(--vgr-line)}#vgr-research .vgr-header h1{color:#000}#vgr-research .vgr-tools,#vgr-research .vgr-jump,#vgr-research .vgr-footer,#vgr-research .vgr-section-nav,#vgr-research .vgr-text-link{display:none!important}#vgr-research .vgr-paper{break-inside:avoid;box-shadow:none}#vgr-research .vgr-paper[hidden],#vgr-research .vgr-paper-section[hidden]{display:block!important}#vgr-research a{color:#000}}
</style>
<div id="vgr-research">
<header class="vgr-header">
<h1>Research</h1>
<p class="vgr-intro">I study how changes in technology and the global economy reshape work, political voice, and democracy. My research asks why similar economic pressures can produce different responses—from support for populist outsiders to political withdrawal or collective action—and how institutions shape who gains, who loses, and who has a say.</p>
</header>
<nav class="vgr-jump" aria-label="Research page sections">
<a href="#research-areas">Research areas</a><a href="#research-publications">Publications & papers</a><a href="#research-public-writing">Public writing</a><a href="https://gonzalez-rostani.com/img/Papers/CV_GonzalezRostani.pdf">Curriculum vitae ↗</a>
</nav>
<section id="research-areas" aria-labelledby="research-areas-title">
<h2 id="research-areas-title">Research areas</h2>
<section class="vgr-area" aria-labelledby="area-01">
<div class="vgr-area-text"><h3 id="area-01">Economic change and political representation</h3><p>I examine how automation, trade, and economic insecurity change people’s political choices. Why do some workers turn to populist outsiders while others disengage or demand greater protection? My research connects these responses to parties’ promises, electoral institutions, and workers’ sense of economic security and social standing. I also trace how technological change crosses borders through trade and production.</p></div>
<div class="vgr-area-papers"><p class="vgr-eyebrow">Selected work</p><ul class="vgr-examples"><li><a href="#paper-political-economic-polarization">Elections, Right-wing Populism, and Political-Economic Polarization: The Role of Institutions and Political Outsiders</a></li><li><a href="#paper-automation-apathy">Engaged Robots, and Disengaged Workers: Automation and Political Apathy</a></li><li><a href="#paper-automation-mexico">The Political Economy of Automation and Fragmented Production in a Global Economy: Evidence from Mexico</a></li><li><a href="#paper-love-of-variety">Love of Variety? An Experimental Study of Heterogeneous Responses to Foreign Brands in the Marketplace</a></li></ul></div>
</section>
<section class="vgr-area" aria-labelledby="area-02">
<div class="vgr-area-text"><h3 id="area-02">AI, work, and who benefits</h3><p>I study how AI changes workers’ everyday experiences and their influence over the future of work. AI can help people perform tasks, replace parts of their jobs, or expand workplace monitoring. I ask how these experiences shape demands for protection and how unions, employers, and public policy determine whether productivity gains translate into better pay, greater autonomy, and economic security.</p></div>
<div class="vgr-area-papers"><p class="vgr-eyebrow">Selected work</p><ul class="vgr-examples"><li><a href="#paper-restoration-politics">From Robot and AI Threats to Restoration Politics: The Role of Perceived Marginalization and Nostalgia</a></li><li><a href="#paper-ai-economy-chapter">AI&#x27;s Economy and Its Political and Institutional Consequences</a></li><li><a href="#paper-machines-manage">When Machines Manage: Workers&#x27; Demands and Trade Union Responses to AI</a></li><li><a href="#paper-ai-augmented-work">The Political Ramifications of AI-Augmented Work</a></li></ul></div>
</section>
<section class="vgr-area" aria-labelledby="area-03">
<div class="vgr-area-text"><h3 id="area-03">Political narratives and methods</h3><p>Understanding political change requires measuring how people explain their experiences and how politicians make their case. I develop tools that use political speech, social media, and open-ended survey responses to study these explanations. My work examines how political narratives differ, how they spread, and how researchers can use AI while assessing the reliability and authorship of the evidence it helps produce.</p></div>
<div class="vgr-area-papers"><p class="vgr-eyebrow">Selected work</p><ul class="vgr-examples"><li><a href="#paper-social-media-surveys">Social Media vs. Surveys: A New Scalable Approach to Understanding Political Discourse</a></li><li><a href="#paper-populist-narratives">Which Populism, Where? Measuring Narrative Strategy at the Sentence Level</a></li><li><a href="#paper-tracing-ai">Measuring Response Authorship in Surveys: An Embedded Experiment to Trace AI Assistance and AI Agents</a></li><li><a href="#paper-immigration-rhetoric">Competing Narratives of Welcome? Migration Shocks and Elite Communication in Chile and Peru</a></li></ul></div>
</section>
</section>
<section id="research-publications" aria-labelledby="research-publications-title">
<div class="vgr-index-heading"><div><p class="vgr-eyebrow">The full index</p><h2 id="research-publications-title">Publications & papers</h2></div><a href="#research-published" class="vgr-text-link">Go to published or forthcoming ↓</a></div>
<p class="vgr-index-note">Journal articles, book chapters, and current projects. Open an abstract for more detail or follow a link to read the paper.</p>
<nav class="vgr-section-nav" aria-label="Publication categories">
<a href="#research-published">Published or forthcoming <span>14</span></a>
<a href="#research-chapters">Book chapters <span>3</span></a>
<a href="#research-review">Papers under review <span>7</span></a>
<a href="#research-working">Working papers <span>3</span></a>
<a href="#research-progress">Selected work in progress <span>5</span></a>
</nav>
<div class="vgr-tools" hidden>
<div class="vgr-search"><label for="vgr-search">Search papers</label><input id="vgr-search" type="search" placeholder="Title, author, journal, or keyword" autocomplete="off"></div>
<div><label for="vgr-topic">Research area</label><select id="vgr-topic"><option value="all">All areas</option><option value="representation">Economic change & representation</option><option value="ai">AI & work</option><option value="methods">Narratives & methods</option><option value="education">Mentoring & inclusion</option></select></div>
<div><label for="vgr-status">Publication status</label><select id="vgr-status"><option value="all">All statuses</option><option value="published">Published or forthcoming</option><option value="chapters">Book chapters</option><option value="review">Papers under review</option><option value="working">Working papers</option><option value="progress">Work in progress</option></select></div>
<button type="button" id="vgr-reset">Reset</button>
<p id="vgr-result-count" role="status" aria-live="polite" aria-atomic="true">Showing all entries</p>
</div>
<p id="vgr-no-results" hidden>No papers match these filters. Try another keyword or reset the filters.</p>
<section class="vgr-paper-section" id="research-published" aria-labelledby="heading-published"><h3 class="vgr-group-title" id="heading-published">Published or forthcoming <span>14</span></h3>
<article class="vgr-paper" id="paper-restoration-politics" data-status="conditional" data-topics="representation ai" aria-labelledby="title-restoration-politics">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-restoration-politics"><a href="https://gonzalez-rostani.com/img/Papers/APSA_Automation_Culture.pdf">From Robot and AI Threats to Restoration Politics: The Role of Perceived Marginalization and Nostalgia</a></h4>
<span class="vgr-badge vgr-badge-conditional">Conditionally accepted</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<p class="vgr-meta"><em>Comparative Political Studies</em></p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/APSA_Automation_Culture.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-restoration-politics" aria-controls="abstract-restoration-politics" aria-expanded="false" hidden>Abstract</button><a href="https://osf.io/3kdpq">Pre-Analysis Plan</a><a href="https://gonzalez-rostani.com/img/Papers/Polmeth_VG.pdf">Poster</a></div>
<details class="vgr-abstract" id="abstract-restoration-politics"><summary>Abstract</summary><div><p>I investigate the impact of automation exposure on political behavior in post-industrial societies, with a specific focus on the support for populism. I examine the potential causal mechanisms by exploring the interplay between economic and cultural factors. Through a parallel encouragement design survey experiment conducted in the US, I divide the sample into two groups: one group is randomly assigned to the treatment condition either related to exposure to robots and AI replacing jobs or a control condition related to technological development; the other group experiences manipulation of both the treatment and the encouragement of mediators (marginalization and nostalgia). My findings reveal that feelings of marginalization and nostalgia mediate the effects of technological change on support for populism and illiberal policies. To enhance external validity, I implement mediation analysis using survey data from the European Social Survey from 2012 to 2016. The results help us understand how structural changes in labor markets and cultural factors impact political behavior and inequality.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-love-of-variety" data-status="published" data-topics="representation" aria-labelledby="title-love-of-variety">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-love-of-variety"><a href="https://www.cambridge.org/core/journals/political-science-research-and-methods/article/love-of-variety-an-experimental-study-of-heterogeneous-responses-to-foreign-brands-in-the-marketplace/B4D9E1CC30B6FC7360552A8E373FAA6A">Love of Variety? An Experimental Study of Heterogeneous Responses to Foreign Brands in the Marketplace</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Jude Hays</p>
<p class="vgr-meta"><em>Political Science Research and Methods</em> · 2026</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://www.cambridge.org/core/journals/political-science-research-and-methods/article/love-of-variety-an-experimental-study-of-heterogeneous-responses-to-foreign-brands-in-the-marketplace/B4D9E1CC30B6FC7360552A8E373FAA6A">Article</a><a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-love-of-variety" aria-controls="abstract-love-of-variety" aria-expanded="false" hidden>Abstract</button><a href="https://osf.io/y8nrm">Pre-Analysis Plan</a><a href="https://gonzalez-rostani.com/img/Papers/APSA_LoV2.pdf">Slides</a></div>
<details class="vgr-abstract" id="abstract-love-of-variety"><summary>Abstract</summary><div><p>This study investigates the impact of exposure to foreign goods in the marketplace on the policy preferences and political behavior of US consumers. Using a survey experiment, we simulate a realistic consumption experience with well-known brands of sports utility vehicles. Our findings reveal that exposure to foreign brands intensifies hostility towards immigrants and trade among respondents holding pre-existing nationalist attitudes while also increasing their support for Trump as a presidential candidate. Exposure to foreign brands has the opposite effect on the preferences and behavior of cosmopolitans. Our results demonstrate that consumption in an increasingly diversified marketplace can drive a bottom-up process of trade policy polarization. Our study has significant implications for understanding the contemporary political backlash against economic globalization and standard models of international trade based on the ``love of variety." </p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-immigration-rhetoric" data-status="conditional" data-topics="representation methods" aria-labelledby="title-immigration-rhetoric">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-immigration-rhetoric"><a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf">Competing Narratives of Welcome? Migration Shocks and Elite Communication in Chile and Peru</a></h4>
<span class="vgr-badge vgr-badge-conditional">Conditionally accepted</span>
</div>
<p class="vgr-authors">With Jose Incio and Guillermo Lezama</p>
<p class="vgr-meta"><em>Legislative Studies Quarterly</em></p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>Narratives &amp; methods</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-immigration-rhetoric" aria-controls="abstract-immigration-rhetoric" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-immigration-rhetoric"><summary>Abstract</summary><div><p>How does an immigration shock affect politicians’ discourses? This study examines the sudden influx of Venezuelan migrants into Latin American countries. We argue that such events alter politicians’ agendas, creating opportunities to frame new issues from their perspectives. Analyzing over 3 million tweets by parliament members from 2013 to 2021 in Chile and Peru, we employ computational textanalysis methods, from simple dictionaries to complex techniques like unsupervised topic analysis and OpenAI, along with an instrumental variable strategy. Our results suggest that after the immigration shock, politicians emphasized the immigration issue without any party family monopolizing it. We find little evidence that regional exposure explains the issue’s salience, suggesting a disconnection from local experiences. Our findings reveal a novel channel for increased salience: right-wing politicians criticized the Venezuelan regime and socialism instead of increasing anti-immigration sentiment, while left-wing politicians promoted pro-immigration attitudes consistent with contact theory. This work enhances our understanding of the politicization of immigration in South-South contexts in the digital age.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-taxing-super-rich" data-status="conditional" data-topics="representation" aria-labelledby="title-taxing-super-rich">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-taxing-super-rich"><a href="https://gonzalez-rostani.com/img/Papers/manuscript_GR_LC.pdf">Can Taxing the Super-Rich Unite Workers? Billionaire Visibility and Coalitional Potential</a></h4>
<span class="vgr-badge vgr-badge-conditional">Conditionally accepted</span>
</div>
<p class="vgr-authors">With Santiago Lopez-Cariboni</p>
<p class="vgr-meta"><em>Latin American Politics and Society</em></p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/manuscript_GR_LC.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-taxing-super-rich" aria-controls="abstract-taxing-super-rich" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-taxing-super-rich"><summary>Abstract</summary><div><p>Extreme wealth has long characterized Latin American democracies, but recently billionaires have become more visible and politically legible targets of taxation. Yet, we know less about how this change translates into coalitional politics among workers divided by labor-market position. We develop a theoretical model in which super-rich visibility raises the perceived fiscal returns from taxing the top and makes divisions within labor appear smaller relative to those at the top. We evaluate its implications using news coverage and documented episodes of mobilization and policy action across Latin America, together with an original Mexican survey pairing closed-ended preferences with open-ended narratives. The evidence documents growing articulation of top-end taxation and shows that support for a targeted top tax extends across partisan groups and is less segmented by labor-market position than support for redistribution that leaves the payer unspecified. Shared fairness claims provide a basis for coordination, while distrust in enforcement and government spending constrains coalition formation.</p><p class="vgr-source"><a href="https://gonzalez-rostani.com/img/Papers/manuscript_GR_LC.pdf">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-environmental-regulation" data-status="published" data-topics="representation" aria-labelledby="title-environmental-regulation">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-environmental-regulation"><a href="https://www.sciencedirect.com/science/article/pii/S0921800926000583">The Threat of Automation and Public Support for Environmental Regulation</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Liam Beiser-McGrath and Michaël Aklin</p>
<p class="vgr-meta"><em>Ecological Economics</em> · 2026</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://www.sciencedirect.com/science/article/pii/S0921800926000583">Article</a><a href="https://gonzalez-rostani.com/img/Papers/Env_automation_EE.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-environmental-regulation" aria-controls="abstract-environmental-regulation" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-environmental-regulation"><summary>Abstract</summary><div><p>In an era of increasing economic precarity and labour market polarization, meaningful efforts to mitigate climate challenges face a fundamental political challenge. We examine how indviduals' long-term labour market risk shapes their environmental attitudes and support for green policies. We argue that long-term labour market risk is expected to reduce environmental concern amongst those affected due to a deprioritization of problems with high levels of uncertainty and that require deep reforms to be addressed. Therefore, we expect labour market risk to subsequently reduce support of environmental policy that imposes immediate direct costs, such as carbon taxation. Using European Social Survey data from 2002 to 2018 and several waves of the International Social Survey Programme across European countries, our analysis reveals that individuals' facing long-term labour market risks are less likely to hold environmental concerns and less supportive of carbon taxes that impose immediate visible costs. Our findings have important implications for understanding how structural transformations in the economy shape individuals' preferences for tackling long-term societal problems like climate change. </p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-sustaining-pathways" data-status="published" data-topics="education" aria-labelledby="title-sustaining-pathways">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-sustaining-pathways"><a href="https://eloncdn.blob.core.windows.net/eu3/sites/923/2026/08/26b14.pdf">Sustaining Pathway Programs in the Social Sciences</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Chie Togami, Tania Ramirez, Fernando Tormos-Aponte, and Yeneca Lee</p>
<p class="vgr-meta"><em>Perspectives on Undergraduate Research &amp; Mentoring</em> · 2026</p>
<div class="vgr-tags"><span>Mentoring &amp; inclusion</span></div>
<div class="vgr-actions"><a href="https://eloncdn.blob.core.windows.net/eu3/sites/923/2026/08/26b14.pdf">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-sustaining-pathways" aria-controls="abstract-sustaining-pathways" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-sustaining-pathways"><summary>Abstract</summary><div><p>Graduate school pathway programs in the social sciences face intensifying political attacks, legal constraints, and defunding. This viewpoint examines strategies for sustaining these programs through strategic reframing, diversified funding, collective knowledge-sharing, and risk-balanced action. It argues that program survival is essential for preserving equity infrastructure and broadening participation in research careers.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-political-economic-polarization" data-status="published" data-topics="representation" aria-labelledby="title-political-economic-polarization">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-political-economic-polarization"><a href="https://www.journals.uchicago.edu/doi/10.1086/734533">Elections, Right-wing Populism, and Political-Economic Polarization: The Role of Institutions and Political Outsiders</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<p class="vgr-meta"><em>The Journal of Politics</em> · 2026</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://www.journals.uchicago.edu/doi/10.1086/734533">Article</a><a href="https://gonzalez-rostani.com/img/Papers/Revised_ms.pdf">Preprint</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-political-economic-polarization" aria-controls="abstract-political-economic-polarization" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-political-economic-polarization"><summary>Abstract</summary><div><p>While there is little doubt that technological change is generating labor market polarization around the world, we know much less about its translation into partisan polarization. I explore the political polarization driven by the rise of right-wing populist parties and leaders throughout developed democracies. I build a theoretical model to explain how right-wing populists have attracted the votes of routine workers, workers exposed to automation risk, and previously loyal to mainstream left-wing parties, within both majoritarian multi-district and multiparty proportional systems. I empirically evaluate the theory, focusing primarily on the US and Germany, using individual vote-switching data and campaign targeting strategies inferred from the content of political speeches and party manifestos.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-graduate-pathways" data-status="conditional" data-topics="education" aria-labelledby="title-graduate-pathways">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-graduate-pathways"><a href="https://gonzalez-rostani.com/img/Papers/MPE2.pdf">Creating Pathways to Graduate Success: Reducing Barriers for Underrepresented Minority Students in the Social Sciences</a></h4>
<span class="vgr-badge vgr-badge-conditional">Conditionally accepted</span>
</div>
<p class="vgr-authors">With Tania Ramirez, Chie Togami, et al.</p>
<p class="vgr-meta"><em>Teaching Sociology</em> · 2026</p>
<div class="vgr-tags"><span>Mentoring &amp; inclusion</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/MPE2.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-graduate-pathways" aria-controls="abstract-graduate-pathways" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-graduate-pathways"><summary>Abstract</summary><div><p>Students from underrepresented populations, including women, first-generation students, and racial and ethnic minorities, face persistent barriers in accessing graduate education and professional development opportunities, particularly in the social sciences. To address these disparities, graduate pipeline programs can provide critical support by providing networking and mentoring opportunities, closing methodological and research skill gaps, and preparing participants to apply to competitive graduate programs. This article outlines the principles and goals of a summer program focused on mobilization and political economy by detailing the rationale, implementation strategies, and evaluation framework used to assess its effects. Evaluation of the inaugural program demonstrated the success of a multilayered mentoring approach, tailored curricula, and comprehensive support structures in fostering participants’ academic growth and career readiness. By highlighting best practices and lessons, we provide a template for institutions seeking to develop initiatives associated with greater diversity in graduate programs in the social sciences, the academic market, and, ultimately, higher education.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-engaging-diversity" data-status="published" data-topics="education" aria-labelledby="title-engaging-diversity">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-engaging-diversity"><a href="https://www.cambridge.org/core/journals/ps-political-science-and-politics/article/engaging-diversity-an-inclusive-approach-to-undergraduate-mentorship-in-mobilization-and-political-economy/EA7BCB1ADDA1E121ABF91F3A9798055C">Engaging Diversity: An Inclusive Approach to Undergraduate Mentorship in Mobilization and Political Economy</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Chie Togami, Mariely Lopez-Santana, Tania Ramirez, Fernando Tormos-Aponte, and Mayra Velez-Serrano</p>
<p class="vgr-meta"><em>PS: Political Science &amp; Politics</em> · 2025</p>
<div class="vgr-tags"><span>Mentoring &amp; inclusion</span></div>
<div class="vgr-actions"><a href="https://www.cambridge.org/core/journals/ps-political-science-and-politics/article/engaging-diversity-an-inclusive-approach-to-undergraduate-mentorship-in-mobilization-and-political-economy/EA7BCB1ADDA1E121ABF91F3A9798055C">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-engaging-diversity" aria-controls="abstract-engaging-diversity" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-engaging-diversity"><summary>Abstract</summary><div><p>The political science discipline faces significant disparities in the representation and participation of underrepresented minorities in graduate education. This lack of diversity among political scientists results in a narrower range of questions being explored within the field. Furthermore, the underrepresentation is particularly pronounced in the political methodology subfield, limiting the scope of tools and perspectives to those predominantly shaped by white scholars. This article proposes a template for teaching and mentoring undergraduate students from underrepresented backgrounds to enhance their opportunities in graduate programs. We examine the Mobilization and Political Economy program, a summer research initiative aimed at minority-serving institutions and underrepresented minorities, designed to equip participants with the tools to study social movements, political mobilization, and structural inequality.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-protest-diffusion" data-status="published" data-topics="representation methods" aria-labelledby="title-protest-diffusion">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-protest-diffusion"><a href="https://www.tandfonline.com/doi/full/10.1080/17457289.2025.2504860">Are Protests Contagious? The Dynamics of Temporal and Spatial Diffusion of Political Protests</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Jeffrey Nonnemacher</p>
<p class="vgr-meta"><em>Journal of Elections, Public Opinion &amp; Parties</em> · 2025</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>Narratives &amp; methods</span></div>
<div class="vgr-actions"><a href="https://www.tandfonline.com/doi/full/10.1080/17457289.2025.2504860">Article</a><a href="https://gonzalez-rostani.com/img/Papers/Protest.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-protest-diffusion" aria-controls="abstract-protest-diffusion" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-protest-diffusion"><summary>Abstract</summary><div><p>Do political protests spread across time and space? While scholars of social movements and political behavior have long debated this question, existing studies often fail to simultaneously account for both spatial and temporal dependencies in protest dynamics. Using protest event analysis and a novel spatiotemporal autoregressive distributed lag (STADL) model, we examine the diffusion of protests across 30 European countries from 2000 to 2015. Our findings provide robust evidence that protests exhibit both temporal and spatial contagion: protest activity in one year significantly increases protest frequency in the following year, and protests in one country contribute to the onset of protests in neighboring states. These results underscore the importance of modeling both dimensions of diffusion to avoid biased inferences and contribute to the broader understanding of protest mobilization. Our study highlights the interconnected nature of political activism and has important implications for research on social movements and political instability.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-automation-apathy" data-status="published" data-topics="representation ai" aria-labelledby="title-automation-apathy">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-automation-apathy"><a href="https://onlinelibrary.wiley.com/doi/10.1111/ecpo.12307">Engaged Robots, and Disengaged Workers: Automation and Political Apathy</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<p class="vgr-meta"><em>Economics &amp; Politics</em> · 2024</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
<p class="vgr-recognition"><a href="https://gonzalez-rostani.com/img/Papers/certificate_top_viewed_article2.pdf">Wiley top-viewed article, 2025</a></p>
<div class="vgr-actions"><a href="https://onlinelibrary.wiley.com/doi/10.1111/ecpo.12307">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-automation-apathy" aria-controls="abstract-automation-apathy" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-automation-apathy"><summary>Abstract</summary><div><p>  This paper investigates the impact of the fourth industrial revolution on politics by proposing a theoretical framework linking technological change with political apathy. Using hierarchical logistic modeling with varying intercepts by country and survey data from the European Social Survey from 2002 to 2018 for 23 European countries, I present evidence that individuals more exposed to technological change are less likely to feel close to a political party, participate in elections and take part in protests. Those individuals exposed to automation are about 10% less likely to be politically engaged than those respondents without exposure to automation risks. I also demonstrate that income levels and unionization rates substantially moderate the direct link between automation and political engagement. The impact of automation on political engagement is smaller among wealthier citizens and in highly unionized environment. The political message from these interaction effects speaks about the reinforcing forces between economic inequality and automation and the role of collective organization. My findings have important implications for understanding automation politics, political inequality, and the demand (or lack of) for protection. </p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-social-media-surveys" data-status="published" data-topics="methods" aria-labelledby="title-social-media-surveys">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-social-media-surveys"><a href="https://onlinelibrary.wiley.com/doi/full/10.1111/lsq.12481">Social Media vs. Surveys: A New Scalable Approach to Understanding Political Discourse</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Jose Incio and Guillermo Lezama</p>
<p class="vgr-meta"><em>Legislative Studies Quarterly</em> · 2024</p>
<div class="vgr-tags"><span>Narratives &amp; methods</span></div>
<p class="vgr-recognition"><a href="https://gonzalez-rostani.com/img/Papers/Top_view_certificate.pdf">Wiley top-viewed article, 2025</a></p>
<div class="vgr-actions"><a href="https://onlinelibrary.wiley.com/doi/full/10.1111/lsq.12481">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-social-media-surveys" aria-controls="abstract-social-media-surveys" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-social-media-surveys"><summary>Abstract</summary><div><p>This paper explores how legislators use social media, specifically investigating whether their posts reflect the concerns expressed by their legislative party peers in an anonymous survey. Utilizing data from Twitter (now X), we compare legislators&#x27; social media posts with their responses in a survey of legislators in Latin America.</p><p>We propose a novel and scalable method for analyzing political communications, employing OpenAI for topic identification in statements and BERTopic analysis to identify clusters of political communication. This approach enables a thorough and detailed examination of these topics over time and across political parties.</p><p>Applying our method to statements made by members of the Chilean Congress, we observe a general alignment between the preferences stated in surveys by elites and the prominence of these issues on Twitter. This result validates social media platforms (particularly Twitter) as a tool for predicting politicians&#x27; preferences. Our methodological approach offers a scalable tool for analyzing political rhetoric over time.</p><p class="vgr-source"><a href="https://onlinelibrary.wiley.com/doi/full/10.1111/lsq.12481">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-moral-economic-ideology" data-status="published" data-topics="representation" aria-labelledby="title-moral-economic-ideology">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-moral-economic-ideology"><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476">Moral and Economic Dimensions of Ideology</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Scott Morgenstern, Elias Chavarria, and Chen Chuang</p>
<p class="vgr-meta"><em>Legislative Studies Quarterly</em> · 2024</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-moral-economic-ideology" aria-controls="abstract-moral-economic-ideology" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-moral-economic-ideology"><summary>Abstract</summary><div><p>Many legislators do not have consistently progressive or conservative policy positions. How does the mix of issue positions relate to the manner in which the legislators consider their placement on the left-right ideological scale? Analyzing data from the Parliamentary Elites in Latin America (PELA) survey, this paper counterposes combinations of legislators’ moral and economic policy positions with their self-located ideological score. Our results confirm the importance of economics, which is consistent with older studies, but we also find that moral issues are at least consistent with – and perhaps germane– to the left-right placement of many of the region’s legislators. Among the findings are that the left is more heterogeneous, especially with respect to moral views, than is the right. We also show that many centrists are closeted conservatives, supporting the “ashamed right” thesis.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-religiosity-article" data-status="published" data-topics="representation" aria-labelledby="title-religiosity-article">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-religiosity-article"><a href="https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923">Legislators&#x27; Religiosity and Same-Sex Marriage in Latin America</a></h4>
<span class="vgr-badge vgr-badge-published">Published</span>
</div>
<p class="vgr-authors">With Scott Morgenstern</p>
<p class="vgr-meta"><em>Latin American Research Review</em> · 2023</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923">Article</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-religiosity-article" aria-controls="abstract-religiosity-article" aria-expanded="false" hidden>Abstract</button><button type="button" class="vgr-disclosure-toggle" data-disclosure="resumen-religiosity-article" aria-controls="resumen-religiosity-article" aria-expanded="false" hidden>Resumen</button></div>
<details class="vgr-abstract" id="abstract-religiosity-article"><summary>Abstract</summary><div><p>Same-sex marriage (SSM) has risen to the top of political agendas across Latin America, but there is also great variance in terms of legal status,  public support, and the policymaking processes.  While the public and social movements have been critical to the advance of SSM, we know little about the views of  those who are directly charged with translating public views into policy: the legislators.  To fill this gap, we utilize a survey of the region’s legislators to first examine the range in support among countries and show how it correlates with legal changes.  We then examine the correlates of legislators’ support for SSM.  While we also test  gender, age, and ideology, our multivariate models focus on religiosity.  We show that in addition to driving support at the  individual level (in the expected direction), religiosity also works as a contextual variable such that having more secular colleagues encourages pious legislators to support same-sex marriage.</p></div></details><details class="vgr-abstract" id="resumen-religiosity-article" lang="es"><summary>Resumen</summary><div><p>El matrimonio entre personas del mismo sexo (MPMS) ha marcado la agenda política en muchos países de América Latina, aunque aún es ilegal en muchos países del continente. No obstante, el apoyo público varía mucho en la región, así como también los roles de los tribunales, presidentes y legislaturas. En este artículo nos enfocamos en los legisladores, ya que son los encargados de representar al público y convertir sus demandas en política pública. Si bien muchas legislaturas han discutido el tema, la literatura no ha examinado de manera intensiva las actitudes de estos representantes hacia el MPMS. Para analizar este fenómeno aplicamos un marco teórico que amplía las teorías basadas en el contexto y contacto social, y utilizamos una encuesta implementada a legisladores en la región para estudiar las variables que correlacionan con el apoyo al MPMS. Si bien también evaluamos variables a nivel individual (tales como género e ideología), nuestros modelos se enfocan en el rol contextual de la religiosidad. Los resultados muestran que tener más colegas seculares alienta a los legisladores, incluso a los creyentes, a apoyar el matrimonio entre personas del mismo sexo.</p></div></details>
</div>
</article>
</section>
<section class="vgr-paper-section" id="research-chapters" aria-labelledby="heading-chapters"><h3 class="vgr-group-title" id="heading-chapters">Book chapters <span>3</span></h3>
<article class="vgr-paper" id="paper-ai-economy-chapter" data-status="chapters" data-topics="ai representation" aria-labelledby="title-ai-economy-chapter">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-ai-economy-chapter"><a href="https://gonzalez-rostani.com/img/Papers/AI_chapter_BBGRS_2026-1-15.docx.pdf">AI&#x27;s Economy and Its Political and Institutional Consequences</a></h4>
<span class="vgr-badge vgr-badge-chapters">Forthcoming</span>
</div>
<p class="vgr-authors">With Carles Boix, Michael Becher, and Daniel Stegmueller</p>
<p class="vgr-meta"><em>Cambridge University Press</em></p>
<p class="vgr-book">In <em>Artificial Intelligence, Politics, and Political Science</em>, edited by Nathaniel Persily and Joshua A. Tucker.</p>
<div class="vgr-tags"><span>AI &amp; work</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/AI_chapter_BBGRS_2026-1-15.docx.pdf">Chapter</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-ai-economy-chapter" aria-controls="abstract-ai-economy-chapter" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-ai-economy-chapter"><summary>Abstract</summary><div><p>We examine the political and institutional consequences of artificial intelligence’s economic impact. Although AI may affect nonroutine jobs in particular, we show that current models about the vulnerability level of occupations and economic sectors differ widely in their forecasts. This may explain why public opinion is not settled about the effects of AI. While many fear AI may displace them from their jobs, a majority seems optimistic about its overall impact. Responses vary, however, by cohort and depending on survey framing. AI’s current training and computing needs have magnified capital concentration and business investment in fixed assets, intensifying the technological sector’s interest in regulatory capture. Taken together, AI’s effects on labor and capital may strain democracy unless a set of policies we outline here are gradually implemented.</p><p class="vgr-source"><a href="https://gonzalez-rostani.com/img/Papers/AI_chapter_BBGRS_2026-1-15.docx.pdf">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-agentic-ai-chapter" data-status="chapters" data-topics="methods" aria-labelledby="title-agentic-ai-chapter">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-agentic-ai-chapter"><a href="https://rohanalexander.github.io/notes_on_the_future/08-Crabtree_Gonzalez_Rostani_Kim.html">Failing Faster, Learning Better: Agentic AI and Empirical Social Science Research</a></h4>
<span class="vgr-badge vgr-badge-chapters">Forthcoming</span>
</div>
<p class="vgr-authors">With Charles Crabtree and Jae Yeon Kim</p>
<p class="vgr-meta"><em>CRC Press</em></p>
<p class="vgr-book">In <em>Notes on the Future of Quantitative Social Science</em>, edited by Rohan Alexander.</p>
<div class="vgr-tags"><span>Narratives &amp; methods</span></div>
<div class="vgr-actions"><a href="https://rohanalexander.github.io/notes_on_the_future/08-Crabtree_Gonzalez_Rostani_Kim.html">Chapter</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-agentic-ai-chapter" aria-controls="abstract-agentic-ai-chapter" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-agentic-ai-chapter"><summary>Abstract</summary><div><p>How can social scientists use agentic AI to produce not more, but better work? We argue that the answer lies in using agentic AI to accelerate iterative search by generating alternatives, testing them, and failing more productively. Drawing on Jonathan Bendor’s framework of innovation as a search problem that balances creativity (broad exploration) and criticism (rigorous evaluation), we organize our chapter around two recurring search failures: creativity failure, in which promising ideas are screened out before they are adequately explored, and criticism failure, in which researchers invest too much in weak research designs. Within that framework, we then discuss two applications. One focuses on organizational-level measurement research, where agentic AI can lower the feasibility barrier to exploring new projects and automate iterative validation, thereby avoiding creativity failure and catching flawed measures before they enter the downstream workflow. Another focus is on experimental research, where the prevalent error might be criticism failure arising from underpowered, under-piloted designs. In this domain, agentic AI enables stress-testing of designs and the implementation of construct validity checks at scale. Though AI agents can be potentially transformative for empirical social science research, we also see key limitations, such as inferences from silicon samples not generalizing to real humans; LLMs defaulting to agreement; AI-generated stimuli carrying biased and multi-barreled treatments; and new problems created by using AI to defend against AI contamination. Agentic AI can be used to improve design, measurement, and validation, but it cannot replace human judgment.</p><p class="vgr-source"><a href="https://rohanalexander.github.io/notes_on_the_future/08-Crabtree_Gonzalez_Rostani_Kim.html">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-religiosity-chapter" data-status="chapters" data-topics="representation" aria-labelledby="title-religiosity-chapter">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-religiosity-chapter"><a href="https://gonzalez-rostani.com/img/Papers/Gonzalez-Rostani_Morgenstern.pdf">Legislators’ Religiosity and Same-Sex Marriage in Latin America</a></h4>
<span class="vgr-badge vgr-badge-chapters">Forthcoming</span>
</div>
<p class="vgr-authors">With Scott Morgenstern</p>
<p class="vgr-meta"><em>Routledge</em></p>
<p class="vgr-book">In <em>The Routledge Handbook of Religion and Politics in Latin America</em>, edited by Dennis P. Petri.</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/Gonzalez-Rostani_Morgenstern.pdf">Chapter</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-religiosity-chapter" aria-controls="abstract-religiosity-chapter" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-religiosity-chapter"><summary>Abstract</summary><div><p>Same-sex marriage has risen to the top of political agendas across Latin America, but it is still illegal in many countries. Public support about the issue varies greatly, and the roles of the courts, presidents, and legislatures have also differed. This article focuses on legislators because they are charged with representing the public and converting demands into policy. Although many legislatures have now voted on the issue, the literature has not intensively examined the policy makers’ attitudes toward same-sex marriage. This study applies a theoretical framework that extends theories considering context and social contact and uses a survey of the region’s legislators to study the correlates of support for same-sex marriage. Although the study also tests for individual-level variables (e.g., gender and ideology), the models focus on the contextual role of religiosity. The results show that having more secular colleagues encourages even pious legislators to support same-sex marriage.</p><p class="vgr-source"><a href="https://gonzalez-rostani.com/img/Papers/Gonzalez-Rostani_Morgenstern.pdf">Abstract source</a></p></div></details>
</div>
</article>
</section>
<section class="vgr-paper-section" id="research-review" aria-labelledby="heading-review"><h3 class="vgr-group-title" id="heading-review">Papers under review <span>7</span></h3>
<article class="vgr-paper" id="paper-navigating-uncertainty" data-status="review" data-topics="ai representation" aria-labelledby="title-navigating-uncertainty">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-navigating-uncertainty"><a href="https://gonzalez-rostani.com/img/Papers/Subjective_Techrisk.pdf">Navigating Uncertainty: How Experience Shapes Perception and Politics in the AI Era</a></h4>
<span class="vgr-badge vgr-badge-review">Revise &amp; resubmit</span>
</div>
<p class="vgr-authors">With Tobias Tober</p>
<p class="vgr-meta"><em>Political Science Research and Methods</em></p>
<div class="vgr-tags"><span>AI &amp; work</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/Subjective_Techrisk.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-navigating-uncertainty" aria-controls="abstract-navigating-uncertainty" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-navigating-uncertainty"><summary>Abstract</summary><div><p>How do individuals perceive technological risk, particularly job insecurity, in the era of AI-driven change? This paper explores how people navigate the uncertainty created by the pace of technology and experts' unclear predictions about its impact on jobs. We focus on three perceptions: techno-optimists, techno-pessimists, and those exposed to rapid technological change, examining their demographic characteristics and implications for political coalition-building. Using data from three original surveys, including open-ended responses, we show that personal and vicarious experiences shape these perceptions, with exposed workers occupying a middle ground between optimism and pessimism. Contrary to the view that high-skilled workers are less vulnerable, we find that perceived employment risks rise with the use of complex technologies like programming languages. Exposed workers and pessimists share political traits, such as support for illiberal policies, while optimists lean toward liberal policies. These results deepen our understanding of how technological risk perceptions influence politics.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-tracing-ai" data-status="review" data-topics="methods ai" aria-labelledby="title-tracing-ai">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-tracing-ai"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6576218">Measuring Response Authorship in Surveys: An Embedded Experiment to Trace AI Assistance and AI Agents</a></h4>
<span class="vgr-badge vgr-badge-review">Reject &amp; resubmit</span>
</div>
<p class="vgr-authors">With Shir Raviv</p>
<p class="vgr-meta"><em>Political Analysis</em></p>
<div class="vgr-tags"><span>Narratives &amp; methods</span><span>AI &amp; work</span></div>
<div class="vgr-actions"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6576218">SSRN</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-tracing-ai" aria-controls="abstract-tracing-ai" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-tracing-ai"><summary>Abstract</summary><div><p>Generative AI creates a measurement problem for survey research. When respondents can outsource summarization, explanation, or fact retrieval, open-ended answers may no longer reflect their own reasoning. We introduce an auditable toolkit that combines response-process paradata with prompt-specific semantic benchmarks to detect AI use in open-ended responses. We validate the approach in a randomized survey experiment in which participants complete a summary task under either blocked AI access or observed access to an embedded AI tool, and by administering the same instrument to a synthetic AI agent. AI-assisted and automated responses leave distinct behavioral and textual traces: they show reduced drafting and revision, greater similarity to AI benchmark output, and lower distinctiveness relative to peer responses. Classifiers built on these signals achieve strong out-of-sample performance. These findings show that, in the age of generative AI, authorship must be measured rather than assumed.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-populist-narratives" data-status="review" data-topics="methods representation" aria-labelledby="title-populist-narratives">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-populist-narratives"><a href="https://gonzalez-rostani.com/img/Papers/Measuring_Populism.pdf">Which Populism, Where? Measuring Narrative Strategy at the Sentence Level</a></h4>
<span class="vgr-badge vgr-badge-review">Under review</span>
</div>
<p class="vgr-authors">With Bree Bang-Jensen and Michael Colaresi</p>
<div class="vgr-tags"><span>Narratives &amp; methods</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/Measuring_Populism.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-populist-narratives" aria-controls="abstract-populist-narratives" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-populist-narratives"><summary>Abstract</summary><div><p>The rise of populism across democracies is one of the greatest challenges to the existing world order since World War II. Yet, we only have very limited tools to measure populism within and across countries. Existing approaches rely on human coding, expert surveys, or dictionary-based analysis and suffer from high costs, low comparability, or low validity. We offer a middle-ground strategy between expensive qualitative reading and coarse machine coding. We extend PULSAR to identify sentences/paragraphs carrying populist narratives by parsing “us” versus “them” frames, who is protecting/threatening “the people,” and other common aspects of political speech. We illustrate the approach with US presidential campaign speeches.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-automation-abroad" data-status="review" data-topics="representation ai" aria-labelledby="title-automation-abroad">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-automation-abroad"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6583578">Automation from Abroad: External Technological Change and the Reorganization of Globalization</a></h4>
<span class="vgr-badge vgr-badge-review">Under review</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
<div class="vgr-actions"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6583578">SSRN</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-automation-abroad" aria-controls="abstract-automation-abroad" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-automation-abroad"><summary>Abstract</summary><div><p>Automation is typically studied as a domestic labor-market shock in advanced economies. This essay argues that, for much of the Global South, it is better understood as a cross-border reorganization of production. Firms deciding where and how to produce compare not only labor and machines within a country, but also offshore labor, migrant labor, and capital-intensive production across jurisdictions. When robotics and AI shift those comparisons in the North, they also reshape trade, reshoring, and political adjustment in economies that have adopted relatively little automation themselves. I call this exposure external automation. The essay makes four claims: foreign automation often matters more than domestic adoption in labor-abundant economies; scholarship on trade and automation still tends to separate technology from trade; adjustment in the South is likely to appear through deindustrialization and weaker labor voice; and automation can widen North-South inequality by concentrating rents, productive capacity, and strategic control in the North.</p><p class="vgr-source"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6583578">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-machines-manage" data-status="review" data-topics="ai representation" aria-labelledby="title-machines-manage">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-machines-manage"><a href="https://gonzalez-rostani.com/img/Papers/Agnolin_GonzalezRostani.pdf">When Machines Manage: Workers&#x27; Demands and Trade Union Responses to AI</a></h4>
<span class="vgr-badge vgr-badge-review">Under review</span>
</div>
<p class="vgr-authors">With Paolo Agnolin</p>
<div class="vgr-tags"><span>AI &amp; work</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://gonzalez-rostani.com/img/Papers/Agnolin_GonzalezRostani.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-machines-manage" aria-controls="abstract-machines-manage" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-machines-manage"><summary>Abstract</summary><div><p>AI and other digital technologies are reshaping work, yet their effects on labor-market institutions are still not well understood. Research on technology and unions has focused largely on robots, leaving open how newer digital tools influence worker organizing and collective bargaining. We argue that technology matters not only because it can replace labor, but because it changes how work is organized. We distinguish among displacement, augmentation, and monitoring technologies, and show that each type affects workplace interaction, job stability, and managerial control in different ways. These changes, in turn, shape both workers demand for collective protection and their ability to organize. They also create different bargaining priorities, including training, shared implementation, limits on surveillance, and job security. We test these ideas with a two-level design. First, using European Social Survey data from 15 countries between 2012 and 2024, we match occupations to emerging technologies and assess links to union membership, working conditions and political attitudes. Second, we analyze over 40,000 Canadian collective agreements from 1993 to 2025 with text analysis and an LLM-based AI exposure measure. Results show varied effects: some technologies raise unionization, while others weaken it and worsen worker outcomes significantly for many employees.</p><p class="vgr-source"><a href="https://gonzalez-rostani.com/img/Papers/Agnolin_GonzalezRostani.pdf">Abstract source</a></p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-ai-augmented-work" data-status="review" data-topics="ai representation" aria-labelledby="title-ai-augmented-work">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-ai-augmented-work"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7142460">The Political Ramifications of AI-Augmented Work</a></h4>
<span class="vgr-badge vgr-badge-review">Under review</span>
</div>
<p class="vgr-authors">With Shir Raviv</p>
<div class="vgr-tags"><span>AI &amp; work</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7142460">SSRN</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-ai-augmented-work" aria-controls="abstract-ai-augmented-work" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-ai-augmented-work"><summary>Abstract</summary><div><p>Recent advances in AI have fueled concerns about future job displacement, prompting research on the political consequences for workers vulnerable to job loss. Yet AI is already deeply embedded in the workplace, shaping the daily experiences of millions who interact with AI software regularly. Large language models (LLMs) are now widely accessible and affordable, enabling workers to adopt them independently. The benefits are immediate: greater efficiency, reduced cognitive effort, and often higher-quality output. But these short-term gains may entail long-term costs. As workers grow dependent on AI, they risk losing essential skills and autonomy. Their use also generates data that improves these tools, inadvertently accelerating automation that could eventually replace them. Do workers recognize these risks, and how do they balance them against short-term benefits in their responses to these changes? We explore these questions using a pre-registered field experiment on an online labor marketplace. We recruited 1,200 workers to perform various tasks, randomizing their (1) access to an AI-assisted tool, (2) the perceived capability of this tool, and (3) the stated long-term objectives of implementing this tool. Using a range of behavioral and attitudinal measures, we track changes in how workers use the AI tool and complete their work over time, as well as their perceived competence, job security, and preferences for policies such as retraining and compensation. By documenting informal resistance strategies through which workers seek to preserve their comparative advantage, our study offers new insight into the political consequences of this technological transformation.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-campaign-influence" data-status="review" data-topics="methods representation" aria-labelledby="title-campaign-influence">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-campaign-influence"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7050058">Who Influences Whom? Analyzing the Interplay of Mainstream and Outsider Parties in Social Media Campaigns</a></h4>
<span class="vgr-badge vgr-badge-review">Under review</span>
</div>
<p class="vgr-authors">With Claudia Salas Gimenez</p>
<div class="vgr-tags"><span>Narratives &amp; methods</span><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7050058">SSRN</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-campaign-influence" aria-controls="abstract-campaign-influence" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-campaign-influence"><summary>Abstract</summary><div><p>Electoral campaigns are high-frequency environments in which parties receive rapid feedback and face immediate incentives to adjust both what they say and how they say it. Yet most research on party competition relies on low-frequency texts, such as manifestos, or on election-to-election change, obscuring strategic adaptation within campaigns. We address this gap by analyzing more than 8,000 YouTube transcripts produced by political parties in Spain and the United Kingdom during the year before elections between 2015 and 2024. Using embeddings, BERT-based measures, dictionaries, and large language models, we develop a general framework for studying campaign communication with social media data. We show that parties adapt ideological positioning as elections approach, shift issue emphasis, and respond selectively to rivals, especially on particular issues and within ideological families, rather than converging uniformly. More broadly, the approach captures movement not only in topics, but also in positions, framing, and rhetorical style.</p></div></details>
</div>
</article>
</section>
<section class="vgr-paper-section" id="research-working" aria-labelledby="heading-working"><h3 class="vgr-group-title" id="heading-working">Working papers <span>3</span></h3>
<article class="vgr-paper" id="paper-automation-mexico" data-status="working" data-topics="representation ai" aria-labelledby="title-automation-mexico">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-automation-mexico"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058">The Political Economy of Automation and Fragmented Production in a Global Economy: Evidence from Mexico</a></h4>
<span class="vgr-badge vgr-badge-working">Working paper</span>
</div>
<p class="vgr-authors">With Carles Boix and Erica Owen</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
<div class="vgr-actions"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058">SSRN</a><a href="https://gonzalez-rostani.com/img/Papers/Automation_developing_MX.pdf">Manuscript</a><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-automation-mexico" aria-controls="abstract-automation-mexico" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-automation-mexico"><summary>Abstract</summary><div><p>How does automation in the Global North shape politics and violence in the Global South? We develop a political economy theory in which robot adoption in advanced economies reduces demand for export-oriented labor in developing countries, depressing wages and employment and creating social and political consequences. We test this argument in Mexico, a close trade partner of the United States. Using commuting-zone data, we construct exposure measures combining pre-NAFTA export employment with U.S. industry robot growth and initial offshoring intensity, while accounting for domestic robot adoption and other shocks. To address endogeneity, we instrument foreign exposure with European robot diffusion. We find that regions more exposed to foreign robots experience higher levels of violent organized crime, including narcocrime and homicides (but not property crime), and stronger support for left-populist candidates. These findings demonstrate how automation shocks ripple through global value chains to reshape society and elections.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-spatial-inla" data-status="working" data-topics="methods" aria-labelledby="title-spatial-inla">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-spatial-inla">Estimating Spatially Structured Cross-Level Effects in Multilevel Models Using INLA</h4>
<span class="vgr-badge vgr-badge-working">Working paper</span>
</div>
<p class="vgr-authors">With Jude Hays</p>
<div class="vgr-tags"><span>Narratives &amp; methods</span></div>
</div>
</article>
<article class="vgr-paper" id="paper-automation-migration" data-status="working" data-topics="representation ai" aria-labelledby="title-automation-migration">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-automation-migration">Automation narrows migration as an adjustment channel in the Mexico–U.S. corridor</h4>
<span class="vgr-badge vgr-badge-working">Working paper</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
<div class="vgr-actions"><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-automation-migration" aria-controls="abstract-automation-migration" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-automation-migration"><summary>Abstract</summary><div><p>This article asks whether automation can close migration as an adjustment mechanism. In the Mexico–U.S. corridor, U.S. robot adoption can reduce mobility through two channels at once: it can lower earnings in Mexican origins by reshoring production and reducing demand for Mexican inputs, and it can weaken labor demand in U.S. destinations. The empirical strategy combines the foreign-robot commuting-zone design developed by Faber (2020) with an extension of the commuting-zone robot design in Acemoglu and Restrepo (2020) to immigrant population outcomes. Mexican commuting zones more exposed to foreign robots have fewer emigrant households and lower emigration intensity, while U.S. commuting zones more exposed to domestic robots experienced smaller increases in Mexico-born population shares between 1990 and 2006–2008. The evidence indicates that automation can narrow exit by reducing realized emigration from origins and migrant absorption in destinations.</p></div></details>
</div>
</article>
</section>
<section class="vgr-paper-section" id="research-progress" aria-labelledby="heading-progress"><h3 class="vgr-group-title" id="heading-progress">Selected work in progress <span>5</span></h3>
<article class="vgr-paper" id="paper-ai-infrastructure" data-status="progress" data-topics="ai" aria-labelledby="title-ai-infrastructure">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-ai-infrastructure">The Political Economy of AI Infraestructure</h4>
<span class="vgr-badge vgr-badge-progress">Work in progress</span>
</div>
<p class="vgr-authors">Valentina González-Rostani</p>
<div class="vgr-tags"><span>AI &amp; work</span></div>
</div>
</article>
<article class="vgr-paper" id="paper-collective-agreements" data-status="progress" data-topics="ai" aria-labelledby="title-collective-agreements">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-collective-agreements">Collective Agreements in the Age of Artificial Intelligence</h4>
<span class="vgr-badge vgr-badge-progress">Work in progress</span>
</div>
<p class="vgr-authors">With Paolo Agnolin</p>
<div class="vgr-tags"><span>AI &amp; work</span></div>
</div>
</article>
<article class="vgr-paper" id="paper-untouchables" data-status="progress" data-topics="representation ai" aria-labelledby="title-untouchables">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-untouchables">The Untouchables: Why We Don&#x27;t Demand Taxes on Big Tech?</h4>
<span class="vgr-badge vgr-badge-progress">Work in progress</span>
</div>
<p class="vgr-authors">With Santiago Lopez-Cariboni</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span><span>AI &amp; work</span></div>
</div>
</article>
<article class="vgr-paper" id="paper-money-talks" data-status="progress" data-topics="representation" aria-labelledby="title-money-talks">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-money-talks">When Money Talks: Rethinking Income Redistribution and Political Inequality</h4>
<span class="vgr-badge vgr-badge-progress">Work in progress</span>
</div>
<p class="vgr-authors">With Jude Hays</p>
<div class="vgr-tags"><span>Economic change &amp; representation</span></div>
<div class="vgr-actions"><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-money-talks" aria-controls="abstract-money-talks" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-money-talks"><summary>Abstract</summary><div><p>Research on the political consequences of economic inequality focuses almost exclusively on relative inequality, using measures such as percentile ratios and gini coefficients. We show with a simple theoretical model that proportionate income increases that preserve relative inequality can increase absolute inequality and generate larger gaps in campaign contributions between rich and poor. Using U.S. congressional district data, we find absolute inequality, rather than relative inequality, is associated with larger contribution gaps.</p></div></details>
</div>
</article>
<article class="vgr-paper" id="paper-networked-approach" data-status="progress" data-topics="education" aria-labelledby="title-networked-approach">
<div class="vgr-paper-body">
<div class="vgr-paper-top">
<h4 id="title-networked-approach">A Networked Approach to Addressing Underrepresentation in the Social and Behavioral Sciences</h4>
<span class="vgr-badge vgr-badge-progress">Work in progress</span>
</div>
<p class="vgr-authors">With Fernando Tormos-Aponte, Chie Togami, Tania Ramirez, Mayra Velez-Serrano, Mariely Lopez-Santana, and Yeneca Lee</p>
<div class="vgr-tags"><span>Mentoring &amp; inclusion</span></div>
<div class="vgr-actions"><button type="button" class="vgr-disclosure-toggle" data-disclosure="abstract-networked-approach" aria-controls="abstract-networked-approach" aria-expanded="false" hidden>Abstract</button></div>
<details class="vgr-abstract" id="abstract-networked-approach"><summary>Abstract</summary><div><p>The current sociopolitical context features growing pressure on higher education inclusion efforts, alongside persistent underrepresentation in the social and behavioral sciences across gender, racialized, ethnic, and socioeconomic lines. Despite decades of initiatives and evidence on the value of diversity, pathway programs that provide mentoring, research experience, and professional socialization to underrepresented student populations often operate in isolation, with uneven funding and limited shared evaluation infrastructure. This Perspective article develops a network model for coordinating pathway programs within and across countries. Drawing on existing consortia and mobility infrastructures, we outline a networked-improvement-community approach that can pool resources, democratize collaborations across institutional types, and support research-informed program design and assessment through a shared Knowledge and Innovation Hub. We use the U.S. landscape as an illustrative case given its program density and policy volatility, while emphasizing design features needed for transnational operation, including shared governance, diversified funding, multilingual access, and context-specific definitions of underrepresentation. By linking existing efforts into a durable alliance, a networked approach aims to expand inclusive pathways into graduate training and research careers in the social sciences and beyond, while increasing resilience in periods of political and fiscal instability.</p></div></details>
</div>
</article>
</section>
</section>
<section id="research-public-writing" aria-labelledby="research-public-writing-title">
<h2 id="research-public-writing-title">Public writing</h2>
<p class="vgr-index-note">Essays bringing these questions to a wider audience.</p>
<ul class="vgr-public-writing">
<li lang="es"><a href="https://www.razonesypersonas.com/2026/09/el-futuro-de-la-inteligencia-artificial.html">El futuro de la inteligencia artificial no está escrito: trabajo, poder y democracia</a><span>September 3, 2026 · Razones y Personas</span></li>
<li lang="es"><a href="https://www.razonesypersonas.com/2025/06/quien-hace-el-trabajo-ahora.html">¿Quién hace el trabajo ahora? Automatización, IA y el desafío del trabajo 4.0</a><span>June 12, 2025 · Razones y Personas</span></li>
<li lang="es"><a href="http://www.razonesypersonas.com/2023/10/la-noche-de-la-nostalgia.html">La noche de la nostalgia</a><span>October 12, 2023 · Razones y Personas</span></li>
<li lang="es"><a href="http://www.razonesypersonas.com/2022/06/todo-robot-es-politico.html">Todo robot es político!</a><span>June 16, 2022 · Razones y Personas</span></li>
</ul></section><footer class="vgr-footer"><a href="#vgr-research">Back to top ↑</a></footer></div>
<script>
(function () {
  'use strict';
  var root = document.getElementById('vgr-research');
  if (!root || root.dataset.ready) return;
  root.dataset.ready = 'true';
  var tools = root.querySelector('.vgr-tools');
  var search = root.querySelector('#vgr-search');
  var topic = root.querySelector('#vgr-topic');
  var status = root.querySelector('#vgr-status');
  var papers = Array.from(root.querySelectorAll('.vgr-paper'));
  var sections = Array.from(root.querySelectorAll('.vgr-paper-section'));
  var result = root.querySelector('#vgr-result-count');
  var empty = root.querySelector('#vgr-no-results');
  // Keep disclosure controls beside the paper links; panels open below the row.
  // Without JavaScript, the original native details/summary controls remain usable.
  root.querySelectorAll('[data-disclosure]').forEach(function (button) {
    var panel = document.getElementById(button.dataset.disclosure);
    if (!panel || !root.contains(panel)) return;
    var summary = panel.querySelector('summary');
    if (!summary) return;
    panel.classList.add('vgr-enhanced');
    summary.hidden = true;
    button.hidden = false;
    function syncDisclosure() {
      button.setAttribute('aria-expanded', String(panel.open));
    }
    button.addEventListener('click', function () {
      panel.open = !panel.open;
      syncDisclosure();
    });
    panel.addEventListener('toggle', syncDisclosure);
    syncDisclosure();
  });
  function normalize(value) {
    return value.normalize('NFD').replace(/[\u0300-\u036f]/g, '').toLowerCase().replace(/[’‘]/g, "'");
  }
  var haystacks = papers.map(function (paper) { return normalize(paper.textContent); });
  function applyFilters() {
    var terms = normalize(search.value).trim().split(/\s+/).filter(Boolean);
    var shown = 0;
    papers.forEach(function (paper, i) {
      var statusMatch = status.value === 'all' || status.value === paper.dataset.status ||
        (status.value === 'published' && paper.dataset.status === 'conditional');
      var match = statusMatch &&
        (topic.value === 'all' || paper.dataset.topics.split(' ').includes(topic.value)) &&
        terms.every(function (term) { return haystacks[i].includes(term); });
      paper.hidden = !match;
      if (match) shown += 1;
    });
    sections.forEach(function (section) {
      var count = section.querySelectorAll('.vgr-paper:not([hidden])').length;
      section.hidden = count === 0;
      section.querySelector('.vgr-group-title span').textContent = count;
    });
    result.textContent = shown === papers.length ? 'Showing all ' + papers.length + ' entries' :
      'Showing ' + shown + ' of ' + papers.length + ' entries';
    empty.hidden = shown !== 0;
  }
  function resetFilters() {
    search.value = '';
    topic.value = 'all';
    status.value = 'all';
    applyFilters();
  }
  function revealTarget(hash, scroll) {
    if (!hash || hash.charAt(0) !== '#') return;
    var target = document.getElementById(hash.slice(1));
    if (!target || !root.contains(target)) return;
    if (target.classList.contains('vgr-paper') || target.classList.contains('vgr-paper-section')) {
      resetFilters();
      if (scroll) target.scrollIntoView({block:'start'});
    }
  }
  search.addEventListener('input', applyFilters);
  topic.addEventListener('change', applyFilters);
  status.addEventListener('change', applyFilters);
  root.querySelector('#vgr-reset').addEventListener('click', function () { resetFilters(); search.focus(); });
  root.addEventListener('click', function (event) {
    var anchor = event.target.closest('a[href^="#"]');
    if (anchor && root.contains(anchor)) revealTarget(anchor.getAttribute('href'), false);
  });
  window.addEventListener('hashchange', function () { revealTarget(window.location.hash, true); });
  tools.hidden = false;
  applyFilters();
  revealTarget(window.location.hash, true);
}());
</script>
