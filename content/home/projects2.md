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
<p>Research on how automation and artificial intelligence reshape politics, labor markets, and democratic institutions, alongside a complementary agenda using NLP and large language models to study political discourse and behavior.</p>
</div>

<div class="controls">
<span class="label">Theme:</span>
<div class="pills">
<button class="pill active" onclick="setTheme('all', this)">All</button>
<button class="pill" onclick="setTheme('automation', this)">Automation & AI</button>
<button class="pill" onclick="setTheme('populism', this)">Populism & Polarization</button>
<button class="pill" onclick="setTheme('methods', this)">Methods</button>
<button class="pill" onclick="setTheme('teaching', this)">Mentoring/Teaching</button>
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

<article class="paper" data-status="published" data-themes="populism automation">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://www.journals.uchicago.edu/doi/10.1086/734533" target="_blank" rel="noopener">Elections, Right-wing Populism, and Political-Economic Polarization: The Role of Institutions and Political Outsiders</a></h3>
<div class="paper-meta"><div><strong>Valentina González-Rostani</strong></div><div><em>The Journal of Politics</em> (2025/2026)</div></div>
<details><summary>Abstract</summary><p>While there is little doubt that technological change is generating labor market polarization around the world, we know much less about its translation into partisan polarization. I explore the political polarization driven by the rise of right-wing populist parties and leaders throughout developed democracies. I build a theoretical model to explain how right-wing populists have attracted the votes of routine workers, workers exposed to automation risk, and previously loyal to mainstream left-wing parties, within both majoritarian multi-district and multiparty proportional systems. I empirically evaluate the theory, focusing primarily on the US and Germany, using individual vote-switching data and campaign targeting strategies inferred from the content of political speeches and party manifestos.</p>
</details> &nbsp; 
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/Revised_ms.pdf>Pre-Print</a> </summary><p> </p>
</details> &nbsp; 
<details><summary><a href=https://www.journals.uchicago.edu/doi/10.1086/734533>First View</a> </summary><p> </p>
<div class="tags"><span class="tag">Automation</span><span class="tag">Populism</span><span class="tag">Text-as-Data</span></div>
</div>
<span class="badge published">Published</span>
</div>
</article>

<article class="paper" data-status="forthcoming" data-themes="trade populism">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf" target="_blank" rel="noopener">Love of Variety? An Experimental Study of Heterogeneous Responses to Foreign Brands in the Marketplace</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://sites.pitt.edu/~jch61/" target="_blank" rel="noopener">Jude C. Hays</a></strong></div><div><em>Conditionally Accepted at Political Science Research and Methods</em> (2026)</div></div>
<details><summary>Abstract</summary><p>This study investigates the impact of exposure to foreign goods in the marketplace on the policy preferences and political behavior of US consumers. Using a survey experiment, we simulate a realistic consumption experience with well-known brands of sports utility vehicles. Our findings reveal that exposure to foreign brands intensifies hostility towards immigrants and trade among respondents holding pre-existing nationalist attitudes while also increasing their support for Trump as a presidential candidate. Exposure to foreign brands has the opposite effect on the preferences and behavior of cosmopolitans. Our results demonstrate that consumption in an increasingly diversified marketplace can drive a bottom-up process of trade policy polarization. Our study has significant implications for understanding the contemporary political backlash against economic globalization and standard models of international trade based on the ``love of variety." </p>
</details> &nbsp; 
<details><summary><a href=https://osf.io/y8nrm>Pre-Analysis Plan</a> </summary><p> </p>
</details> &nbsp; 
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/APSA_LoV2.pdf>Slides</a> </summary><p> </p>
</details> &nbsp;   
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf>Manuscript</a> </summary><p> </p>  
</details> &nbsp; <br>
<div class="tags"><span class="tag">Trade</span><span class="tag">Experiment</span></div>
</div>
<span class="badge forthcoming">Accepted</span>
</div>
</article>

<article class="paper" data-status="published" data-themes="teaching">
<div class="paper-top">
<div>
<h3 class="paper-title"><a href="https://cup.org/4ibfZqa" target="_blank" rel="noopener">Engaging Diversity: An Inclusive Approach to Undergraduate Mentorship in Mobilization and Political Economy</a></h3>
<div class="paper-meta"><div><strong>with <a href="https://chietogami.com/" target="_blank" rel="noopener">Chie Togami</a>, <a href="https://marielylopezsantana.weebly.com/" target="_blank" rel="noopener">Mariely Lopez-Santana</a>, Tania Ramirez, <a href="https://www.fernandotormos.com/" target="_blank" rel="noopener">Fernando Tormos-Aponte</a>, and Mayra Velez-Serrano</strong></div><div><em>PS: Political Science & Politics</em> (2025)</div></div>
<details><summary>Abstract</summary><p>The political science discipline faces significant disparities in the representation and participation of underrepresented minorities in graduate education. This lack of diversity among political scientists results in a narrower range of questions being explored within the field. Furthermore, the underrepresentation is particularly pronounced in the political methodology subfield, limiting the scope of tools and perspectives to those predominantly shaped by white scholars. This article proposes a template for teaching and mentoring undergraduate students from underrepresented backgrounds to enhance their opportunities in graduate programs. We examine the Mobilization and Political Economy program, a summer research initiative aimed at minority-serving institutions and underrepresented minorities, designed to equip participants with the tools to study social movements, political mobilization, and structural inequality.</p>
</details> &nbsp; 
<details><summary><a href=https://cup.org/4ibfZqa>First View</a> </summary><p> </p>
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
<details><summary>Abstract</summary><p>Do political protests spread across time and space? While scholars of social movements and political behavior have long debated this question, existing studies often fail to simultaneously account for both spatial and temporal dependencies in protest dynamics. Using protest event analysis and a novel spatiotemporal autoregressive distributed lag (STADL) model, we examine the diffusion of protests across 30 European countries from 2000 to 2015. Our findings provide robust evidence that protests exhibit both temporal and spatial contagion: protest activity in one year significantly increases protest frequency in the following year, and protests in one country contribute to the onset of protests in neighboring states. These results underscore the importance of modeling both dimensions of diffusion to avoid biased inferences and contribute to the broader understanding of protest mobilization. Our study highlights the interconnected nature of political activism and has important implications for research on social movements and political instability.</p>
</details> &nbsp; 
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/Protest.pdf>Manuscript</a> </summary><p> </p>
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
<details><summary>Abstract</summary><p>Many legislators do not have consistently progressive or conservative policy positions. How does the mix of issue positions relate to the manner in which the legislators consider their placement on the left-right ideological scale? Analyzing data from the Parliamentary Elites in Latin America (PELA) survey, this paper counterposes combinations of legislators’ moral and economic policy positions with their self-located ideological score. Our results confirm the importance of economics, which is consistent with older studies, but we also find that moral issues are at least consistent with – and perhaps germane– to the left-right placement of many of the region’s legislators. Among the findings are that the left is more heterogeneous, especially with respect to moral views, than is the right. We also show that many centrists are closeted conservatives, supporting the “ashamed right” thesis.</p>
</details> &nbsp; 
<details><summary><a href=https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476>First View</a> </summary><p> </p>
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
<details><summary>Abstract</summary><p>  This paper investigates the impact of the fourth industrial revolution on politics by proposing a theoretical framework linking technological change with political apathy. Using hierarchical logistic modeling with varying intercepts by country and survey data from the European Social Survey from 2002 to 2018 for 23 European countries, I present evidence that individuals more exposed to technological change are less likely to feel close to a political party, participate in elections and take part in protests. Those individuals exposed to automation are about 10% less likely to be politically engaged than those respondents without exposure to automation risks. I also demonstrate that income levels and unionization rates substantially moderate the direct link between automation and political engagement. The impact of automation on political engagement is smaller among wealthier citizens and in highly unionized environment. The political message from these interaction effects speaks about the reinforcing forces between economic inequality and automation and the role of collective organization. My findings have important implications for understanding automation politics, political inequality, and the demand (or lack of) for protection. </p>
</details> &nbsp; 
<details><summary><a href=http://doi.org/10.1111/ecpo.12307 >First View</a> </summary><p> </p>
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
<details><summary>Abstract</summary><p>Many legislators do not have consistently progressive or conservative policy positions. How does the mix of issue positions relate to the manner in which the legislators consider their placement on the left-right ideological scale? Analyzing data from the Parliamentary Elites in Latin America (PELA) survey, this paper counterposes combinations of legislators’ moral and economic policy positions with their self-located ideological score. Our results confirm the importance of economics, which is consistent with older studies, but we also find that moral issues are at least consistent with – and perhaps germane– to the left-right placement of many of the region’s legislators. Among the findings are that the left is more heterogeneous, especially with respect to moral views, than is the right. We also show that many centrists are closeted conservatives, supporting the “ashamed right” thesis.</p>
</details> &nbsp; 
<details><summary><a href=https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476>First View</a> </summary><p> </p>
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
<details><summary>Abstract</summary><p>Same-sex marriage (SSM) has risen to the top of political agendas across Latin America, but there is also great variance in terms of legal status,  public support, and the policymaking processes.  While the public and social movements have been critical to the advance of SSM, we know little about the views of  those who are directly charged with translating public views into policy: the legislators.  To fill this gap, we utilize a survey of the region’s legislators to first examine the range in support among countries and show how it correlates with legal changes.  We then examine the correlates of legislators’ support for SSM.  While we also test  gender, age, and ideology, our multivariate models focus on religiosity.  We show that in addition to driving support at the  individual level (in the expected direction), religiosity also works as a contextual variable such that having more secular colleagues encourages pious legislators to support same-sex marriage.</p>
</details> &nbsp; 
<details><summary>Resumen</summary><p>El matrimonio entre personas del mismo sexo (MPMS) ha marcado la agenda política en muchos países de América Latina, aunque aún es ilegal en muchos países del continente. No obstante, el apoyo público varía mucho en la región, así como también los roles de los tribunales, presidentes y legislaturas. En este artículo nos enfocamos en los legisladores, ya que son los encargados de representar al público y convertir sus demandas en política pública. Si bien muchas legislaturas han discutido el tema, la literatura no ha examinado de manera intensiva las actitudes de estos representantes hacia el MPMS. Para analizar este fenómeno aplicamos un marco teórico que amplía las teorías basadas en el contexto y contacto social, y utilizamos una encuesta implementada a legisladores en la región para estudiar las variables que correlacionan con el apoyo al MPMS. Si bien también evaluamos variables a nivel individual (tales como género e ideología), nuestros modelos se enfocan en el rol contextual de la religiosidad. Los resultados muestran que tener más colegas seculares alienta a los legisladores, incluso a los creyentes, a apoyar el matrimonio entre personas del mismo sexo.</p>
</details> &nbsp; 
<details><summary><a href=https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923#article>First View</a> </summary><p> </p>
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

<div class="paper-meta">
<div><strong>with <a href="https://www.princeton.edu/~cboix/" target="_blank" rel="noopener">Carles Boix</a> and <a href="https://www.polisci.pitt.edu/people/erica-owen" target="_blank" rel="noopener">Erica Owen</a></strong></div>
<div><em>Working Paper</em> (2025)</div>
</div>

<details><summary>Abstract</summary><div><p>How does automation in the Global North shape politics and violence in the Global South? We develop a political economy theory in which robot adoption in advanced economies reduces demand for export-oriented labor in developing countries, depressing wages and employment and creating social and political consequences. We test this argument in Mexico, a close trade partner of the United States. Using commuting-zone data, we construct exposure measures combining pre-NAFTA export employment with U.S. industry robot growth and initial offshoring intensity, while accounting for domestic robot adoption and other shocks. To address endogeneity, we instrument foreign exposure with European robot diffusion. We find that regions more exposed to foreign robots experience higher levels of violent organized crime, including narcocrime and homicides (but not property crime), and stronger support for left-populist candidates. These findings demonstrate how automation shocks ripple through global value chains to reshape society and elections.</p></div></details>

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
<details><summary>Abstract</summary><p>How do individuals perceive technological risk, particularly job insecurity, in the era of AI-driven change? This paper explores how people navigate the uncertainty created by the pace of technology and experts' unclear predictions about its impact on jobs. We focus on three perceptions: techno-optimists, techno-pessimists, and those exposed to rapid technological change, examining their demographic characteristics and implications for political coalition-building. Using data from three original surveys, including open-ended responses, we show that personal and vicarious experiences shape these perceptions, with exposed workers occupying a middle ground between optimism and pessimism. Contrary to the view that high-skilled workers are less vulnerable, we find that perceived employment risks rise with the use of complex technologies like programming languages. Exposed workers and pessimists share political traits, such as support for illiberal policies, while optimists lean toward liberal policies. These results deepen our understanding of how technological risk perceptions influence politics.</p>
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
<details><summary>Abstract</summary><p> The rise of automation has transformed economies around the world. We examine how its effects spill over and affect people's views about environmental issues and policies. We argue that the long-term economic threat posed by automation is expected to reduce environmental concern amongst those affected due to a deprioritization of problems with high levels of uncertainty and that require deep reforms to be addressed. Therefore, we expect automation risk to subsequently reduce support of environmental policy that imposes immediate direct costs, such as carbon taxation. Meanwhile, support for policies with diffuse costs, such as environmental subsidies, will only be affected by automation indirectly, to the extent that it reduces individuals' general environmental concern. Using European Social Survey data from 2002 to 2018 for 23 European countries, our analysis reveals that individuals exposed to automation are less likely to hold environmental concerns and less supportive of carbon taxes that impose immediate visible costs. Mediation analysis suggests that automation reduces support for environmental policies through its negative effect on environmental concern,  with this effect being larger for subsidies. Our findings have important implications for understanding how structural transformations in the economy shape individuals' preferences for tackling long-term societal problems like climate change.</p>
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
<details><summary>Abstract</summary><p>How does an immigration shock affect politicians’ discourses? This study examines the sudden influx of Venezuelan migrants into Latin American countries. We argue that such events alter politicians’ agendas, creating opportunities to frame new issues from their perspectives. Analyzing over 3 million tweets by parliament members from 2013 to 2021 in Chile and Peru, we employ computational textanalysis methods, from simple dictionaries to complex techniques like unsupervised topic analysis and OpenAI, along with an instrumental variable strategy. Our results suggest that after the immigration shock, politicians emphasized the immigration issue without any party family monopolizing it. We find little evidence that regional exposure explains the issue’s salience, suggesting a disconnection from local experiences. Our findings reveal a novel channel for increased salience: right-wing politicians criticized the Venezuelan regime and socialism instead of increasing anti-immigration sentiment, while left-wing politicians promoted pro-immigration attitudes consistent with contact theory. This work enhances our understanding of the politicization of immigration in South-South contexts in the digital age.</p> </details> &nbsp; 
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">Latin America</span><span class="tag">Immigration</span><span class="tag">Text-as-Data</span></div>
</div>
<span class="badge under-review">Under Review</span>
</div>
</article>

<!-- The path from Automation to Populist Political Behavior -->
<article class="paper" data-status="working" data-themes="automation populism methods">
<div class="paper-top">
<div>
<h3 class="paper-title">The path from Automation to Populist Political Behavior</h3>
<div class="paper-meta"><div><strong>Valentina González-Rostani</strong></div><div><em>Working Paper</em> (2023) · Presented at APSA 2022, IPES 2022, EUSA 2023, EPSA 2023, PolMeth XL, APSA 2023, Virtual IPES 2024, Yale · To be presented at Caltech</div></div>
<details><summary>Abstract</summary><p>I investigate the impact of automation exposure on political behavior in post-industrial societies, with a specific focus on the support for populism. I examine the potential causal mechanisms by exploring the interplay between economic and cultural factors. Through a parallel encouragement design survey experiment conducted in the US, I divide the sample into two groups: one group is randomly assigned to the treatment condition either related to exposure to robots and AI replacing jobs or a control condition related to technological development; the other group experiences manipulation of both the treatment and the encouragement of mediators (marginalization and nostalgia). My findings reveal that feelings of marginalization and nostalgia mediate the effects of technological change on support for populism and illiberal policies. To enhance external validity, I implement mediation analysis using survey data from the European Social Survey from 2012 to 2016. The results help us understand how structural changes in labor markets and cultural factors impact political behavior and inequality.</p>
</details> &nbsp; 
<details><summary><a href=https://osf.io/3kdpq>Pre-Analysis Plan</a> </summary><p> </p>
</details> &nbsp; 
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/Polmeth_VG.pdf>Poster</a> </summary><p> </p>
</details> &nbsp; 
<details><summary><a href=https://gonzalez-rostani.com/img/Papers/APSA_Automation_Culture.pdf>Manuscript</a> </summary><p> </p>
<div class="tags"><span class="tag">Automation</span><span class="tag">Populism</span><span class="tag">Experiment</span><span class="tag">Mediation</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Who Influences Whom -->
<article class="paper" data-status="working" data-themes="populism methods">
<div class="paper-top">
<div>
<h3 class="paper-title">Who Influences Whom? Analyzing the Interplay of Mainstream and Outsider Parties in Social Media Campaigns</h3>
<div class="paper-meta"><div><strong>Valentina González-Rostani</strong></div><div><em>Working Paper</em> (2024)</div></div>
<details><summary>Abstract</summary><p>Do mainstream parties respond to outsider parties, or vice versa? Previous research suggests an alignment between the issues prioritized by both mainstream and outsider parties, but definitive evidence on who influences whom is limited. I investigate this with fine-grained temporal analyses of YouTube videos posted by political parties in the year leading up to elections since 2015 in the UK and Spain. Using dictionaries, Wordscores, and transformer-based models, I classify the content by issues and communication characteristics, such as whether a message is populist or extreme. I then apply vector autoregression models to explore short-term dynamics of rhetorical influence. In the UK, a majoritarian system, mainstream right and left parties respond to each other, while the outsider right follows mainstream parties. In Spain, a multi-party system, mainstream parties influence each other, and outsider parties influence the mainstream left and each other. More importantly, in both systems, mainstream parties more often lead than follow outsiders' messages. These findings have important implications for understanding party dynamics and competition during electoral campaigns.</p>
<div class="tags"><span class="tag">Campaigns</span><span class="tag">YouTube</span><span class="tag">VAR</span><span class="tag">Text-as-Data</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Creating Pathways to Graduate Success -->
<article class="paper" data-status="under-review" data-themes="teaching">
<div class="paper-top">
<div>
<h3 class="paper-title">Creating Pathways to Graduate Success: Reducing Barriers for Underrepresented Minority Students in the Social Sciences</h3>
<div class="paper-meta"><div><strong>with <a href="https://chietogami.com/" target="_blank" rel="noopener">Chie Togami</a>, <a href="https://marielylopezsantana.weebly.com/" target="_blank" rel="noopener">Mariely Lopez-Santana</a>, Tania Ramirez, <a href="https://www.fernandotormos.com/" target="_blank" rel="noopener">Fernando Tormos-Aponte</a>, and Mayra Velez-Serrano</strong></div><div><em>Under Review</em></div></div>
<details><summary>Abstract</summary><p>Students from underrepresented populations, including women, first-generation students, and racial and ethnic minorities, face persistent barriers in accessing graduate education and professional development opportunities, particularly in the social sciences. To address these disparities, graduate pipeline programs can provide critical support by providing networking and mentoring opportunities, closing methodological and research skill gaps, and preparing participants to apply to competitive graduate programs. This article outlines the principles and goals of a summer program focused on mobilization and political economy by detailing the rationale, implementation strategies, and evaluation framework used to assess its effects. Evaluation of the inaugural program demonstrated the success of a multilayered mentoring approach, tailored curricula, and comprehensive support structures in fostering participants’ academic growth and career readiness. By highlighting best practices and lessons, we provide a template for institutions seeking to develop initiatives associated with greater diversity in graduate programs in the social sciences, the academic market, and, ultimately, higher education.</p> </details> &nbsp; 
<details><summary><a href="https://gonzalez-rostani.com/img/Papers/MPE2.pdf" target="_blank" rel="noopener">Manuscript</a></summary><div><p>PDF.</p></div></details>
<div class="tags"><span class="tag">Mentorship</span><span class="tag">Pipeline Programs</span><span class="tag">Equity</span></div>
</div>
<span class="badge under-review">Under Review</span>
</div>
</article>

<!-- Spatiotemporal approach -->
<article class="paper" data-status="working" data-themes="methods">
<div class="paper-top">
<div>
<h3 class="paper-title">A Spatiotemporal Approach to Model Multilevel Data Structures</h3>
<div class="paper-meta"><div><strong>with <a href="https://sites.pitt.edu/~jch61/" target="_blank" rel="noopener">Jude C. Hays</a></strong></div><div><em>Working Paper</em> (2023) · Presented at APSA 2023</div></div>
<details><summary>Abstract</summary><p>The analysis of multilevel data is common in political science and the social sciences more generally. We examine the case where random community-level effects cluster geographically in space. Ignoring this spatial dependence leads to inefficient coefficient estimates and overconfident standard errors. We propose a two-step spatial feasible generalized least squares estimator that, under empirically identifiable conditions, provides relatively efficient coefficient estimates and accurate standard errors compared to the maximum likelihood estimation of non-spatial models.</p>
<details><summary>Draft Upon Request</summary><div><p>Please send me an email, and I will share our most recent working paper.</p></div></details>
<div class="tags"><span class="tag">Spatial</span><span class="tag">Multilevel</span><span class="tag">FGLS</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- AI-Augmented Work -->
<article class="paper" data-status="working" data-themes="automation">
<div class="paper-top">
<div>
<h3 class="paper-title">The Political Ramification of AI-Augmented Work: Evidence from a Field Experiment</h3>
<div class="paper-meta"><div><strong>with <a href="https://www.ravivshir.net/" target="_blank" rel="noopener">Shir Raviv</a></strong></div><div><em>Working Paper</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>Recent advances in AI have fueled concerns about future job displacement, prompting research on the political consequences for workers vulnerable to job loss. Yet AI is already deeply embedded in the workplace, shaping the daily experiences of millions who interact with AI software regularly. Large language models (LLMs) are now widely accessible and affordable, enabling workers to adopt them independently. The benefits are immediate: greater efficiency, reduced cognitive effort, and often higher-quality output. But these short-term gains may entail long-term costs. As workers grow dependent on AI, they risk losing essential skills and autonomy. Their use also generates data that improves these tools, inadvertently accelerating automation that could eventually replace them. Do workers recognize these risks, and how do they balance them against short-term benefits in their responses to these changes? We explore these questions using a pre-registered field experiment on an online labor marketplace. We recruited 1,200 workers to perform various tasks, randomizing their (1) access to an AI-assisted tool, (2) the perceived capability of this tool, and (3) the stated long-term objectives of implementing this tool. Using a range of behavioral and attitudinal measures, we track changes in how workers use the AI tool and complete their work over time, as well as their perceived competence, job security, and preferences for policies such as retraining and compensation. By documenting informal resistance strategies through which workers seek to preserve their comparative advantage, our study offers new insight into the political consequences of this technological transformation.</p></div></details>
<div class="tags"><span class="tag">AI</span><span class="tag">Field Experiment</span><span class="tag">Labor</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Detecting AI-Generated Responses -->
<article class="paper" data-status="working" data-themes="methods automation">
<div class="paper-top">
<div>
<h3 class="paper-title">Detecting AI-Generated Responses in Surveys: A Behavioral–Linguistic Toolkit</h3>
<div class="paper-meta"><div><strong>with <a href="https://www.ravivshir.net/" target="_blank" rel="noopener">Shir Raviv</a></strong></div><div><em>Working Paper</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>The rapid adoption of large language models (LLMs) has introduced a new form of survey misrepresentation: respondents using AI to craft their answers. Traditional fraud checks and text-only classifiers fail to detect such behavior reliably, allowing synthetic content to contaminate datasets. This research note presents a behavioral–linguistic toolkit for identifying AI-generated survey responses. The toolkit integrates three components—front-end copy-paste blocking, keystroke-dynamics monitoring, and post-hoc linguistic analysis combining embeddings, perplexity, and AI-similarity scores. We validate this approach in a randomized online experiment comparing “AI-Allowed” and “AI-Blocked” conditions. Results show clear behavioral and textual signatures of AI use: longer and more fluent answers with minimal editing, high semantic overlap with model-generated text, and reduced typing variability. These indicators jointly predict AI use with high accuracy, outperforming existing detection methods. The proposed framework offers a scalable solution for preserving data quality and transparency in the era of generative AI, providing a foundation for future best practices in survey methodology.</p></div></details>
<div class="tags"><span class="tag">Survey Methods</span><span class="tag">LLMs</span><span class="tag">Detection</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Too Rich to Tax -->
<article class="paper" data-status="working" data-themes="trade">
<div class="paper-top">
<div>
<h3 class="paper-title">Too Rich to Tax? Technological Elites, Economic Inequality, and Public Attitudes Toward Taxing the Super-Rich</h3>
<div class="paper-meta"><div><strong>with <a href="https://lopez-cariboni.info/" target="_blank" rel="noopener">Santiago Lopez-Cariboni</a></strong></div><div><em>Working Paper</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>This project investigates the societal, cultural, and psychological factors that give rise to this belief in “impossibility” and discusses the implications for policy-making and advocacy. Through survey experiments, we examine how collective skepticism prevents citizens from demanding reform, and we also explore the role of perceived state capacity in reinforcing the notion that taxing high-net-worth individuals is unrealistic. By uncovering the roots of this mindset, our study seeks to explain why so many people in developing nations refrain from voicing support for wealth taxation—even though inequality is widely recognized. Ultimately, this research aims to reframe the conversation around tax justice on a global scale, offering practical steps and policy recommendations to dismantle the barriers of disbelief.</p></div></details>
<details><summary><a href="https://osf.io/k3ypc/files/kznsb" target="_blank" rel="noopener">PAP</a></summary><div><p>OSF.</p></div></details>
<div class="tags"><span class="tag">Inequality</span><span class="tag">Tax</span><span class="tag">Survey Experiments</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- AI and the Future of Democracy -->
<article class="paper" data-status="working" data-themes="automation">
<div class="paper-top">
<div>
<h3 class="paper-title">Artificial Intelligence and the Future of Democracy: Political and Institutional Consequences of Economic Dislocation</h3>
<div class="paper-meta"><div><strong>with <a href="https://www.princeton.edu/~cboix/" target="_blank" rel="noopener">Carles Boix</a></strong></div><div><em>Working Paper / Review</em> (2025)</div></div>
<details><summary>Abstract</summary><div><p>The rapid advancement of artificial intelligence (AI) is reshaping economies, labor markets, and political landscapes, raising urgent questions about its implications for democracy. This paper reviews the growing body of research on the political and institutional consequences of AI-driven economic dislocation. While AI-induced automation threatens traditional employment structures, its effects on political participation, electoral behavior, and policy preferences remain less understood. Existing evidence suggests that economic insecurity caused by automation can fuel political dissatisfaction and increase support for populist and anti-establishment movements. At the same time, AI-driven growth creates economic winners who may reinforce existing political alignments. However, the ways in which voters perceive and respond to AI-induced economic change—whether through policy demands, shifts in ideological preferences, or institutional trust—remain contested. This review highlights key theoretical perspectives, synthesizes recent empirical findings, and identifies pressing questions for future research on the intersection of AI, economic dislocation, and democratic stability.</p></div></details>
<div class="tags"><span class="tag">AI</span><span class="tag">Democracy</span><span class="tag">Political Economy</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Populist PULSAR -->
<article class="paper" data-status="working" data-themes="populism methods">
<div class="paper-top">
<div>
<h3 class="paper-title">You Can't Stop It If You Can't See It: Introducing a New Scalable System to Measure Populist Narratives at Higher Resolution</h3>
<div class="paper-meta"><div><strong>with <a href="https://www.breebangjensen.com/" target="_blank" rel="noopener">Bree Bang-Jensen</a> and <a href="https://michaelcolaresi.com/" target="_blank" rel="noopener">Michael Colaresi</a></strong></div><div><em>Working Paper</em> (2025) · Presented at ISA 2024, MPSA 2025</div></div>
<details><summary>Abstract</summary><div><p>The rise of populism across democracies is one of the greatest challenges to the existing world order since World War II. Yet, we only have very limited tools to measure populism within and across countries. Existing approaches rely on human coding, expert surveys, or dictionary-based analysis and suffer from high costs, low comparability, or low validity. We offer a middle-ground strategy between expensive qualitative reading and coarse machine coding. We extend PULSAR to identify sentences/paragraphs carrying populist narratives by parsing “us” versus “them” frames, who is protecting/threatening “the people,” and other common aspects of political speech. We illustrate the approach with US presidential campaign speeches.</p></div></details>
<div class="tags"><span class="tag">Populism</span><span class="tag">NLP</span><span class="tag">Measurement</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

<!-- Sustaining Pathway Programs in the Social Sciences -->
<article class="paper" data-status="under-review" data-themes="teaching">
<div class="paper-top">
<div>
<h3 class="paper-title">Sustaining Pathway Programs in the Social Sciences</h3>
<div class="paper-meta"><div><strong>with <a href="https://chietogami.com/" target="_blank" rel="noopener">Chie Togami</a>, <a href="https://marielylopezsantana.weebly.com/" target="_blank" rel="noopener">Yeneca Lee</a>, Tania Ramirez, <a href="https://www.fernandotormos.com/" target="_blank" rel="noopener">, and Fernando Tormos-Aponte</a></strong></div><div><em>Under Review</em></div></div>
</div>

<details>
<summary>Abstract</summary>
<div><p>Graduate school pathway programs in the social sciences face intensifying political attacks, legal constraints, and defunding. This viewpoint examines strategies for sustaining these programs through strategic reframing, diversified funding, collective knowledge-sharing, and risk-balanced action. It argues that program survival is essential for preserving equity infrastructure and broadening participation in research careers.</p></div>
</details>

<div class="tags">
<span class="tag">Pathway Programs</span>
<span class="tag">DEI</span>
<span class="tag">Higher Education</span>
<span class="tag">Academic Freedom</span>
</div>
</div>

<span class="badge working">Viewpoint</span>
</div>
</article>


<!-- When Money Talks -->
<article class="paper" data-status="working" data-themes="populism">
<div class="paper-top">
<div>
<h3 class="paper-title">When Money Talks: Rethinking Income Redistribution and Political Inequality</h3>
<div class="paper-meta"><div><strong>with <a href="https://sites.pitt.edu/~jch61/" target="_blank" rel="noopener">Jude C. Hays</a></strong></div><div><em>Working Paper</em> (2025) · Presented at Vienna University (2022)</div></div>
<details><summary>Abstract</summary><div><p>Research on the political consequences of economic inequality focuses almost exclusively on relative inequality, using measures such as percentile ratios and gini coefficients. We show with a simple theoretical model that proportionate income increases that preserve relative inequality can increase absolute inequality and generate larger gaps in campaign contributions between rich and poor. Using U.S. congressional district data, we find absolute inequality, rather than relative inequality, is associated with larger contribution gaps.</p></div></details>
<div class="tags"><span class="tag">Inequality</span><span class="tag">Political Finance</span><span class="tag">Theory + Evidence</span></div>
</div>
<span class="badge working">Working</span>
</div>
</article>

</div>

<hr class="hr"/>

<h2 class="section-title">Diffusion</h2>



<div class="grid">
<article class="paper" data-status="published" data-themes="automation">
<h3 class="paper-title"><a href="https://www.razonesypersonas.com/2025/06/quien-hace-el-trabajo-ahora.html" target="_blank" rel="noopener">¿Quién hace el trabajo ahora? Automatización, IA y el desafío del trabajo 4.0</a></h3>
<div class="paper-meta">June 12, 2025 · Razones y Personas</div>
</article>
  


<article class="paper" data-status="published" data-themes="populism">
<h3 class="paper-title"><a href="http://www.razonesypersonas.com/2023/10/la-noche-de-la-nostalgia.html" target="_blank" rel="noopener">La noche de la nostalgia</a></h3>
<div class="paper-meta">October 12, 2023 · Razones y Personas</div>
</article>

<div class="grid">
<article class="paper" data-status="published" data-themes="automation">
<h3 class="paper-title"><a href="http://www.razonesypersonas.com/2022/06/todo-robot-es-politico.html" target="_blank" rel="noopener">Todo robot es político!</a></h3>
<div class="paper-meta">June 16, 2022 · Razones y Personas</div>
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
