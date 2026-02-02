---
title: 
layout: docs  # Do not modify.
---

<style>
/* HERO BOX (Teaching) */
.teaching-hero{
text-align:center;
margin:0 0 26px;
padding:28px 18px;
background:linear-gradient(135deg,#667eea 0%,#764ba2 100%);
border-radius:18px;
color:#fff
}
.teaching-hero h1{
font-family:inherit;
font-size:2.1em;
font-weight:800;
margin:0 0 10px
}
.teaching-hero p{
font-size:1.05em;
opacity:.95;
max-width:980px;
margin:0 auto;
line-height:1.6
}

/* FILTER BAR (Courses) */
.course-controls{display:flex;gap:12px;flex-wrap:wrap;align-items:center;margin:14px 0 18px}
.course-controls .label{font-weight:800;color:#1f2937}
.course-pills{display:flex;gap:10px;flex-wrap:wrap}
.course-pill{padding:8px 14px;border-radius:999px;border:2px solid #e5e7eb;background:#fff;cursor:pointer;font-weight:800;font-size:.92em;transition:all .2s ease;user-select:none}
.course-pill:hover{border-color:#667eea}
.course-pill.active{background:#667eea;border-color:#667eea;color:#fff}
.course-card.hidden{display:none}
/* END FILTER BAR */

/* COURSE CARD (match research-style feel) */
.course-box{
background:#fff;
border:1px solid #e5e7eb;
border-radius:14px;
padding:18px;
box-shadow:0 2px 10px rgba(0,0,0,.04);
transition:all .2s ease;
margin:12px 0 18px
}
.course-box:hover{
box-shadow:0 8px 24px rgba(0,0,0,.08);
transform:translateY(-1px)
}
.course-title{
margin:0 0 6px;
font-weight:800
}
.course-meta{
color:#6b7280;
font-size:.98em;
margin:0 0 12px
}

/* BUTTONS (like research page) */
.course-actions{display:flex;gap:10px;flex-wrap:wrap;margin:6px 0 0}
.action-btn{
display:inline-block;
padding:8px 12px;
border-radius:8px;
border:1px solid #b21619;
color:#b21619;
text-decoration:none !important;
font-weight:800;
font-size:.9em;
transition:all .2s ease;
background:#fff
}
.action-btn:hover{
background:#b21619;
color:#fff
}
/* optional: secondary buttons (blue) */
.action-btn.blue{
border-color:#3b82f6;
color:#2563eb
}
.action-btn.blue:hover{
background:#3b82f6;
color:#fff
}

/* Summary toggle (kept as details, but styled cleanly) */
.course-details{margin-top:10px}
.course-details summary{
list-style:none;
display:inline-block;
padding:8px 12px;
border-radius:8px;
border:1px solid #b21619;
color:#b21619;
font-weight:800;
cursor:pointer;
user-select:none
}
.course-details summary::-webkit-details-marker{display:none}
.course-details summary:hover{background:#b21619;color:#fff}
.course-details .panel{
margin-top:10px;
padding:12px 14px;
border:1px solid #e5e7eb;
border-radius:10px;
background:#fff
}
.course-details .panel p{margin:0;color:#374151;line-height:1.65}
</style>

<div class="teaching-hero">
<h1>Teaching</h1>
<p>My teaching focused on building strong analytical foundations in methods and political economy, combining hands-on data analysis, computational tools, and substantive theory to help students reason critically about politics, markets, and inequality.</p>
</div>

# ✏️ Courses  

<div class="course-controls">
<span class="label">Level:</span>
<div class="course-pills">
<button class="course-pill active" data-kind="level" onclick="setCourseLevel('all', this)">All</button>
<button class="course-pill" data-kind="level" onclick="setCourseLevel('grad', this)">🎓 Graduate</button>
<button class="course-pill" data-kind="level" onclick="setCourseLevel('undergrad', this)">🧑‍🎓 Undergraduate</button>
</div>
</div>

<div class="course-controls">
<span class="label">Topic:</span>
<div class="course-pills">
<button class="course-pill active" data-kind="topic" onclick="setCourseTopic('all', this)">All</button>
<button class="course-pill" data-kind="topic" onclick="setCourseTopic('methods', this)">📊 Methods</button>
<button class="course-pill" data-kind="topic" onclick="setCourseTopic('ipe', this)">🌍 IPE</button>
</div>
</div>

<script>
let courseLevel='all';
let courseTopic='all';

function setActive(kind, el){
document.querySelectorAll('.course-pill[data-kind="'+kind+'"]').forEach(b=>b.classList.remove('active'));
if(el) el.classList.add('active');
}
function setCourseLevel(level, el){
courseLevel=level; setActive('level', el); applyCourseFilters();
}
function setCourseTopic(topic, el){
courseTopic=topic; setActive('topic', el); applyCourseFilters();
}
function applyCourseFilters(){
document.querySelectorAll('.course-card').forEach(card=>{
const lvl=card.dataset.level || '';
const topics=(card.dataset.topics || '').split(' ').filter(Boolean);
const okLevel=(courseLevel==='all') || (lvl===courseLevel);
const okTopic=(courseTopic==='all') || (topics.includes(courseTopic));
card.classList.toggle('hidden', !(okLevel && okTopic));
});
}
</script>

<!-- POIR612 -->
<article class="course-card" data-level="grad" data-topics="methods">
<div class="course-box">
<h4 class="course-title">POIR612 - Text as Data for Social Scientists 🤖</h4>
<div class="course-meta">📍 <em>University of Southern California</em>, Fall 2025</div>

<div class="course-actions">
<a class="action-btn" href="https://colab.research.google.com/drive/1YMkoWyMPIHYvRtw5RLlUnJ7wxDdVodfv?usp=sharing" target="_blank" rel="noopener">📄 Syllabus</a>
<a class="action-btn blue" href="https://www.notion.so/Text-as-Data-for-Social-Science-Classroom-Home-23510fb8267980cd8571c44bbae73eff?source=copy_link" target="_blank" rel="noopener">🌐 Course Website</a>
</div>

<details class="course-details">
<summary>📖 Summary</summary>
<div class="panel"><p>The course introduces social scientists to computational techniques for analyzing large-scale textual information. Bridging NLP, machine learning, Bayesian statistics, and the social sciences, it emphasizes practical applications in political discourse analysis, sentiment detection, and policy communication. Students learn preprocessing, text representation (bag-of-words, embeddings), supervised learning, topic models, and modern transformer/LLM approaches, alongside ethical and methodological considerations.</p></div>
</details>
</div>
</article>

<!-- IR312 -->
<article class="course-card" data-level="undergrad" data-topics="methods">
<div class="course-box">
<h4 class="course-title">IR312 - Intro to Data Analysis 📊</h4>
<div class="course-meta">📍 <em>University of Southern California</em>, Spring 2026</div>

<div class="course-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/Methods_Spring2026.pdf" target="_blank" rel="noopener">📄 Syllabus</a>
</div>

<details class="course-details">
<summary>📖 Summary</summary>
<div class="panel"><p>How can we measure income inequality? What predicts election outcomes? Do policy interventions reduce poverty? This course equips students with tools to analyze data, draw statistical inferences, and apply causal reasoning to real-world political, social, and economic questions. No prior statistical background is required.</p></div>
</details>
</div>
</article>

<!-- IR430 -->
<article class="course-card" data-level="undergrad" data-topics="ipe">
<div class="course-box">
<h4 class="course-title">IR430 - The Politics of International Trade 🌍</h4>
<div class="course-meta">📍 <em>University of Southern California</em>, Spring 2026</div>

<div class="course-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/IPE_Spring2026.pdf" target="_blank" rel="noopener">📄 Syllabus</a>
</div>

<details class="course-details">
<summary>📖 Summary</summary>
<div class="panel"><p>This course examines the political economy of international trade, connecting foundational theories and debates to contemporary issues. Students analyze how trade policies are made, who benefits and loses, and how global economic shifts shape domestic politics and international cooperation.</p></div>
</details>
</div>
</article>

<!-- MPE Quant Methods -->
<article class="course-card" data-level="undergrad" data-topics="methods ipe">
<div class="course-box">
<h4 class="course-title">Mobilization and Political Economy, Quantitative Methods Course 📢</h4>
<div class="course-meta">📍 <em>NSF-REU Summer Research Program</em>, Summer 2023</div>

<div class="course-actions">
<a class="action-btn blue" href="https://www.migapprogram.com/" target="_blank" rel="noopener">🌐 MPE Website</a>
</div>

<details class="course-details">
<summary>📖 Program summary</summary>
<div class="panel"><p>The MPE Summer Program is an eight-week, in-residence research and mentoring initiative funded by NSF (REU Award #2150250). It supports underrepresented and first-generation undergraduates—especially from MSIs—through methodological training and structured guidance for graduate applications, connecting theory to hands-on data work.</p></div>
</details>

<details class="course-details">
<summary>📖 Course summary</summary>
<div class="panel"><p>The Quantitative Methods course builds a foundation in research design, descriptive statistics, and regression, then advances to hypothesis testing and multi-level modeling. Students learn R programming through real datasets (e.g., CMPS and census data), strengthening skills in data management, modeling, and applied policy analysis.</p></div>
</details>
</div>
</article>

<!-- PS0700 -->
<article class="course-card" data-level="undergrad" data-topics="methods">
<div class="course-box">
<h4 class="course-title">PS0700 - Research Methods in Political Science ⚙️</h4>
<div class="course-meta">📍 <em>University of Pittsburgh</em>, Summer 2022</div>

<div class="course-actions">
<a class="action-btn" href="https://www.dropbox.com/s/shpfv8m1ke1iyr3/PS0700_S22.pdf?dl=0" target="_blank" rel="noopener">📄 Syllabus</a>
</div>

<details class="course-details">
<summary>📖 Summary</summary>
<div class="panel"><p>This course builds students’ ability to understand and conduct quantitative political science research. Emphasis is on data analysis, inference, and causal reasoning, preparing students to interpret research methods used in academic work, policy memos, and social science reporting. No prior statistics required.</p></div>
</details>
</div>
</article>

# 🎤 Guest Lectures  

- _Mobilization and Political Economy_ NSF-REU Summer Camp: **The Political Economy of Automation**, Summer 2025.  
- _Political Economy of Growth_ (PS2543), University of Pittsburgh. **Technological Change and Automation of Jobs**, Spring 2023.  
- _Mobilization and Political Economy_ NSF-REU Summer Camp: **Theories of Political Economy**, Summer 2023.  

Slides available upon request. 

<br>
