+++
widget = "blank"
headless = true
active = true
weight = 26

title = "Research"
subtitle = ""

[design]
  columns = "1"

[design.spacing]
  padding = ["40px", "0", "40px", "0"]
+++

<style>
@import url('https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600;700&family=Work+Sans:wght@400;500;600&display=swap');
.research-container{max-width:1100px;margin:0 auto;font-family:'Work Sans',sans-serif}
.research-hero{text-align:center;margin-bottom:28px;padding:28px 18px;background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);border-radius:18px;color:#fff}
.research-hero h1{font-family:'Crimson Pro',serif;font-size:2.3em;font-weight:700;margin:0 0 10px}
.research-hero p{font-size:1.05em;opacity:.95;max-width:900px;margin:0 auto;line-height:1.6}
.section-title{font-family:'Crimson Pro',serif;font-size:1.9em;font-weight:700;margin:34px 0 18px;color:#1f2937;border-bottom:3px solid #667eea;padding-bottom:8px;display:inline-block}
.controls{display:flex;gap:10px;flex-wrap:wrap;align-items:center;margin:10px 0 18px}
.controls .label{font-weight:700;color:#1f2937;margin-right:6px}
.pills{display:flex;gap:10px;flex-wrap:wrap}
.pill{padding:8px 14px;border-radius:999px;border:2px solid #e5e7eb;background:#fff;cursor:pointer;font-weight:700;font-size:.9em;transition:all .2s ease;user-select:none}
.pill:hover{border-color:#667eea}
.pill.active{background:#667eea;border-color:#667eea;color:#fff}
.grid{display:grid;gap:18px}
.paper{background:#fff;border:1px solid #e5e7eb;border-left:5px solid #e5e7eb;border-radius:14px;padding:18px;box-shadow:0 2px 10px rgba(0,0,0,.04);transition:all .2s ease}
.paper:hover{border-left-color:#667eea;box-shadow:0 8px 24px rgba(0,0,0,.08);transform:translateX(4px)}
.paper.hidden{display:none}
.paper-top{display:flex;justify-content:space-between;gap:14px;align-items:flex-start;margin-bottom:10px}
.paper-title{font-family:'Crimson Pro',serif;font-size:1.2em;font-weight:700;line-height:1.35;margin:0}
.paper-title a{text-decoration:none;color:#111827}
.paper-title a:hover{color:#667eea}
.paper-meta{color:#6b7280;font-size:.95em;line-height:1.45;margin-top:6px}
.badge{padding:6px 12px;border-radius:999px;font-weight:800;font-size:.8em;white-space:nowrap}
.badge.published{background:#c6f6d5;color:#22543d}
.badge.forthcoming{background:#bee3f8;color:#1e3a8a}
.badge.under-review{background:#feebc8;color:#7c2d12}
.badge.working{background:#e5e7eb;color:#111827}
.tags{display:flex;gap:8px;flex-wrap:wrap;margin:10px 0 0}
.tag{padding:4px 10px;border-radius:999px;background:#f3f4f6;border:1px solid #e5e7eb;color:#111827;font-weight:700;font-size:.78em}
details{display:inline-block;margin:8px 10px 0 0;vertical-align:top}
details > summary{list-style:none;display:inline-block;margin:0;padding:6px 10px;color:#b21619;border:1px solid #b21619;border-radius:8px;cursor:pointer;font-weight:800;font-size:.85em;user-select:none}
details > summary:hover{color:#fff;background:#b21619}
details > summary::-webkit-details-marker{display:none}
details > div{margin-top:8px;padding:10px 12px;border:1px solid #e5e7eb;border-radius:10px;background:#fff;box-shadow:0 1px 6px rgba(0,0,0,.06);max-width:900px}
details p{margin:0;color:#374151;line-height:1.6}
.hr{height:1px;background:#e5e7eb;border:0;margin:22px 0}
@media(max-width:768px){.paper-top{flex-direction:column}.research-hero h1{font-size:1.9em}}
</style>

<div class="research-container">
<div class="research-hero">
<h1>Research</h1>
<p>Publications, working papers, and selected projects on automation & AI, political behavior, political methodology, and Latin American politics.</p>
</div>

<div class="controls">
<span class="label">Theme:</span>
<div class="pills">
<button class="pill active" onclick="setTheme('all', this)">All</button>
<button class="pill" onclick="setTheme('automation', this)">Automation & AI</button>
<button class="pill" onclick="setTheme('populism', this)">Populism & Polarization</button>
<button class="pill" onclick="setTheme('methods', this)">Methods</button>
<button class="pill" onclick="setTheme('latin-america', this)">Latin America</button>
<button class="pill" onclick="setTheme('trade', this)">Trade & Labor</button>
</div>
</div>

<div class="controls">
<span class="label">Status:</span>
<div class="pills">
<button class="pill active" onclick="setStatus('all', this)">All</button>
<button class="pill" onclick="setStatus('published', this)">Published</button>
<button class="pill" onclick="setStatus('forthcoming', this)">Forthcoming / Accepted</button>
<button class="pill" onclick="setStatus('under-review', this)">Under Review</button>
<button class="pill" onclick="setStatus('working', this)">Working Papers</button>
</div>
</div>

<hr class="hr"/>

<h2 class="section-title">Publications</h2>

<div class="grid" id="papers">

<article class="paper" data-status="published" data-themes="populism automation methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://www.journals.uchicago.edu/doi/10.1086/734533" target="_blank" rel="noopener">Elections, Right-wing Populism, and Political-Economic Polarization: The Role of Institutions and Political Outsiders</a></h3>
<div class="paper-meta"><div><strong>Valentina González-Rostani</strong></div><div><em>The Journal of Politics</em> (2025/2026)</div></div>
<details><summary>Abstract</summary><div><p>While there is little doubt that technological change is generating labor market polarization around the world, we know much less about its translation into partisan polarization. I explore the political polarization driven by the rise of right-wing populist parties and leaders throughout developed democracies. I build a theoretical model to explain how right-wing populists have attracted the votes of routine workers, workers exposed to automation risk, and previously loyal to mainstream left-wing parties, within both majoritarian multi-district and multiparty proportional systems. I empirically evaluate the theory, focusing primarily on the US and Germany, using individual vote-switching data and campaign targeting strategies inferred from the content of political speeches and party manifestos.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/Revised_ms.pdf" target="_blank" rel="noopener">Pre-Print</a></summary><div><p>PDF.</p></div></details>
<details><summary><a href="https://www.journals.uchicago.edu/doi/10.1086/734533" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Automation</span><span class="tag">Populism</span><span class="tag">Text-as-Data</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="forthcoming" data-themes="trade methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf" target="_blank" rel="noopener">Love of Variety? An Experimental Study of Heterogeneous Responses to Foreign Brands in the Marketplace</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://sites.pitt.edu/~jch61/" target="_blank" rel="noopener">Jude C. Hays</a></strong></div><div><em>Conditionally Accepted at Political Science Research and Methods</em> (2026)</div></div>
<details><summary>Abstract</summary><div><p>This study investigates the impact of exposure to foreign goods in the marketplace on the policy preferences and political behavior of US consumers. Using a survey experiment, we simulate a realistic consumption experience with well-known brands of sports utility vehicles. Our findings reveal that exposure to foreign brands intensifies hostility towards immigrants and trade among respondents holding pre-existing nationalist attitudes while also increasing their support for Trump as a presidential candidate. Exposure to foreign brands has the opposite effect on the preferences and behavior of cosmopolitans. Our results demonstrate that consumption in an increasingly diversified marketplace can drive a bottom-up process of trade policy polarization.</p></div></details>
<details><summary><a href="https://osf.io/y8nrm" target="_blank" rel="noopener">Pre-Analysis Plan</a></summary><div><p>OSF.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/APSA_LoV2.pdf" target="_blank" rel="noopener">Slides</a></summary><div><p>PDF.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">Trade</span><span class="tag">Experiment</span></div>
</div>
<span class="badge forthcoming">Accepted</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://cup.org/4ibfZqa" target="_blank" rel="noopener">Engaging Diversity: An Inclusive Approach to Undergraduate Mentorship in Mobilization and Political Economy</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://chietogami.com/" target="_blank" rel="noopener">Chie Togami</a>, <a href="https://marielylopezsantana.weebly.com/" target="_blank" rel="noopener">Mariely Lopez-Santana</a>, Tania Ramirez, <a href="https://www.fernandotormos.com/" target="_blank" rel="noopener">Fernando Tormos-Aponte</a>, and Mayra Velez-Serrano</strong></div><div><em>PS: Political Science & Politics</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>The political science discipline faces significant disparities in the representation and participation of underrepresented minorities in graduate education. This article proposes a template for teaching and mentoring undergraduate students from underrepresented backgrounds to enhance their opportunities in graduate programs, drawing on the Mobilization and Political Economy program.</p></div></details>
<details><summary><a href="https://cup.org/4ibfZqa" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Mentorship</span><span class="tag">Methods</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="populism methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://www.tandfonline.com/doi/abs/10.1080/17457289.2025.2504860" target="_blank" rel="noopener">Are Protests Contagious? The Dynamics of Temporal and Spatial Diffusion of Political Protests</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://www.jeffreynonnemacher.com/" target="_blank" rel="noopener">Jeffrey Nonnemacher</a></strong></div><div><em>Journal of Elections, Public Opinion & Parties</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>Do political protests spread across time and space? Using protest event analysis and a spatiotemporal autoregressive distributed lag model across 30 European countries (2000–2015), we find robust evidence of both temporal and spatial diffusion.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/Protest.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">Diffusion</span><span class="tag">Spatial</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="methods latin-america">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481" target="_blank" rel="noopener">Social Media versus Surveys: A New Scalable Approach to Understanding Political Discourse</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://joseincio.com/" target="_blank" rel="noopener">Jose Luis Incio</a> and <a href="https://guillelezama.netlify.app/" target="_blank" rel="noopener">Guillermo Lezama</a></strong></div><div><em>Legislative Studies Quarterly</em> (2024)</div></div>
<details><summary>Abstract</summary><div><p>This paper explores whether legislators’ social media posts reflect concerns stated by their party peers in an anonymous survey. Using Twitter and PELA, we propose a scalable method using OpenAI-based topic identification and BERTopic to track political issues across time and parties.</p></div></details>
<details><summary><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Text-as-Data</span><span class="tag">Latin America</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="automation">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="http://doi.org/10.1111/ecpo.12307" target="_blank" rel="noopener">Engaged Robots, and Disengaged Workers: Automation and Political Apathy</a></h3>
<div class="paper-meta"><div><strong>Valentina González-Rostani</strong></div><div><em>Economics & Politics</em> (2024)</div></div>
<details><summary>Abstract</summary><div><p>This paper links technological change to political apathy. Using European Social Survey data (2002–2018) and hierarchical models across 23 countries, I show that workers exposed to automation are about 10% less likely to be politically engaged, with income and unionization moderating the effect.</p></div></details>
<details><summary><a href="http://doi.org/10.1111/ecpo.12307" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Automation</span><span class="tag">Political Behavior</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="latin-america">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476" target="_blank" rel="noopener">How Germane are Moral and Economic Policies to Ideology? Evidence from Latin American Legislators</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://chavarriamora.com/" target="_blank" rel="noopener">Elias Chavarria</a>, Chuang Chen, and <a href="https://smorgens.wixsite.com/website" target="_blank" rel="noopener">Scott Morgenstern</a></strong></div><div><em>Legislative Studies Quarterly</em> (2024)</div></div>
<details><summary>Abstract</summary><div><p>Using PELA, this paper links legislators’ moral and economic policy positions to their self-placement on the left–right scale, showing that economics matters but moral issues are also germane for many legislators. The left is more heterogeneous (especially on moral views), and many centrists appear “closeted conservatives.”</p></div></details>
<details><summary><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Latin America</span><span class="tag">Ideology</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="latin-america">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923" target="_blank" rel="noopener">Legislators’ Religiosity and Same-Sex Marriage in Latin America</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://smorgens.wixsite.com/website" target="_blank" rel="noopener">Scott Morgenstern</a></strong></div><div><em>Latin American Research Review</em> (2023)</div></div>
<details><summary>Abstract</summary><div><p>Using a survey of legislators in Latin America, we examine cross-national variation in support for same-sex marriage and show how religiosity shapes support at the individual level and contextually: more secular colleagues encourage even pious legislators to support SSM.</p></div></details>
<details><summary>Resumen</summary><div><p>El matrimonio entre personas del mismo sexo ha marcado la agenda política en América Latina. Analizamos actitudes legislativas y mostramos el rol contextual de la religiosidad: tener más colegas seculares alienta a legisladores, incluso creyentes, a apoyar el MPMS.</p></div></details>
<details><summary><a href="https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923" target="_blank" rel="noopener">First View</a></summary><div><p>Publisher page.</p></div></details>
<div class="tags"><span class="tag">Latin America</span><span class="tag">Religion</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

</div>

<h2 class="section-title">Working papers & selected work in progress</h2>

<div class="grid">

<article class="paper" data-status="working" data-themes="automation trade latin-america">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058" target="_blank" rel="noopener">The Political Economy of Automation and Fragmented Production: Evidence from Mexico</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://www.princeton.edu/~cboix/" target="_blank" rel="noopener">Carles Boix</a> and <a href="https://www.polisci.pitt.edu/people/erica-owen" target="_blank" rel="noopener">Erica Owen</a></strong></div><div><em>Working Paper</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>How does automation in the Global North shape politics and violence in the Global South? Using Mexico, we show that U.S. robot adoption reduces demand for export-oriented labor and is associated with higher levels of violent organized crime and stronger support for left-populist candidates. The findings illustrate how automation shocks ripple through global value chains.</p></div></details>
<details><summary><a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058" target="_blank" rel="noopener">Manuscript</a></summary><div><p>SSRN.</p></div></details>
<div class="tags"><span class="tag">Automation</span><span class="tag">Trade</span><span class="tag">Latin America</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<article class="paper" data-status="under-review" data-themes="automation methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://gonzalez-rostani.com/img/Papers/Subjective_Techrisk.pdf" target="_blank" rel="noopener">Navigating Uncertainty: How Experience Shapes Perception and Politics in the AI Era</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://tobiastober.github.io/" target="_blank" rel="noopener">Tobias Tober</a></strong></div><div><em>Under Review</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>How do individuals perceive technological risk in the era of AI? Using original surveys (including open-ended responses), we show that personal and vicarious experience shapes techno-optimism/pessimism and perceived job risk, with “exposed” workers occupying a middle ground but sharing some political traits with pessimists.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/Subjective_Techrisk.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">AI</span><span class="tag">Risk</span><span class="tag">Survey</span></div>
</div>
<span class="badge under-review">Under Review</span>
</div>
</article>

<article class="paper" data-status="under-review" data-themes="automation">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://osf.io/esm98/" target="_blank" rel="noopener">The Threat of Automation and Public Support for Environmental Policies</a></h3>
<div class="paper-meta"><div><strong>with <a href="http://www.liambeisermcgrath.com/" target="_blank" rel="noopener">Liam F. Beiser-McGrath</a> and <a href="https://michaelaklin.github.io/" target="_blank" rel="noopener">Michaël Aklin</a></strong></div><div><em>Under Review</em> (2022)</div></div>
<details><summary>Abstract</summary><div><p>We argue automation risk reduces environmental concern and support for costly environmental policies, especially carbon taxation. Using ESS data (2002–2018) across 23 countries, we find exposed individuals are less environmentally concerned and less supportive of carbon taxes; mediation analysis suggests concern explains much of the effect.</p></div></details>
<details><summary><a href="https://osf.io/esm98/" target="_blank" rel="noopener">Manuscript</a></summary><div><p>OSF.</p></div></details>
<div class="tags"><span class="tag">Automation</span><span class="tag">Environment</span></div>
</div>
<span class="badge under-review">Under Review</span>
</div>
</article>

<article class="paper" data-status="under-review" data-themes="latin-america methods">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf" target="_blank" rel="noopener">Immigration Shocks and Politicians’ Rhetoric: Evidence from The Venezuelan Migration Crisis</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://joseincio.com/" target="_blank" rel="noopener">Jose Luis Incio</a> and <a href="https://guillelezama.netlify.app/" target="_blank" rel="noopener">Guillermo Lezama</a></strong></div><div><em>Under Review</em> (2023)</div></div>
<details><summary>Abstract</summary><div><p>Analyzing over 3 million tweets by MPs in Chile and Peru (2013–2021), we show how the Venezuelan migration shock reshaped agendas without one party family monopolizing the issue. Right-wing politicians emphasized regime/socialism critiques, while left-wing politicians promoted pro-immigration stances consistent with contact theory.</p></div></details>
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">Latin America</span><span class="tag">Immigration</span><span class="tag">Text-as-Data</span></div>
</div>
<span class="badge under-review">Under Review</span>
</div>
</article>

</div>

<hr class="hr"/>

<h2 class="section-title">Diffusion</h2>

<div class="grid">
<article class="paper" data-status="published" data-themes="automation">
<h3 class="paper-title"><a href="http://www.razonesypersonas.com/2022/06/todo-robot-es-politico.html" target="_blank" rel="noopener">Todo robot es político!</a></h3>
<div class="paper-meta">June 16, 2022 · Razones y Personas</div>
</article>

<article class="paper" data-status="published" data-themes="populism">
<h3 class="paper-title"><a href="http://www.razonesypersonas.com/2023/10/la-noche-de-la-nostalgia.html" target="_blank" rel="noopener">La noche de la nostalgia</a></h3>
<div class="paper-meta">October 12, 2023 · Razones y Personas</div>
</article>
</div>

</div>

<script>
let currentTheme = 'all';
let currentStatus = 'all';

function clearActives(kind){
const btns = document.querySelectorAll('button.pill[data-kind="'+kind+'"]');
btns.forEach(b => b.classList.remove('active'));
}

function setTheme(theme, el) {
currentTheme = theme;
document.querySelectorAll('.controls').forEach(()=>{});
document.querySelectorAll('.controls .pills button').forEach(b=>{
if(b.getAttribute('data-kind')==='theme') b.classList.remove('active');
});
if(el) el.classList.add('active');
applyFilters();
}

function setStatus(status, el) {
currentStatus = status;
document.querySelectorAll('.controls .pills button').forEach(b=>{
if(b.getAttribute('data-kind')==='status') b.classList.remove('active');
});
if(el) el.classList.add('active');
applyFilters();
}

function applyFilters() {
document.querySelectorAll('.paper').forEach(card => {
const cardStatus = card.dataset.status || '';
const cardThemes = (card.dataset.themes || '').split(' ').filter(Boolean);
const statusOK = (currentStatus === 'all') || (cardStatus === currentStatus);
const themeOK = (currentTheme === 'all') || (cardThemes.includes(currentTheme));
card.classList.toggle('hidden', !(statusOK && themeOK));
});
}
</script>
