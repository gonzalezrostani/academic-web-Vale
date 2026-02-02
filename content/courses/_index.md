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

/* COURSE CARD (paper-like) */
.course-box{
background:#fff;
border:1px solid #e5e7eb;
border-radius:16px;
padding:22px 22px 18px;
box-shadow:0 2px 10px rgba(0,0,0,.05);
transition:all .2s ease;
margin:12px 0 22px;
position:relative;
overflow:hidden;
}
.course-box:hover{
box-shadow:0 10px 28px rgba(0,0,0,.10);
transform:translateY(-1px);
}

/* left accent bar like research cards */
.course-box::before{
content:"";
position:absolute;
left:0;
top:0;
bottom:0;
width:6px;
background:#a7b7ff;
}

/* TOP ROW: title/meta on left, badge on right */
.course-top{
display:flex;
justify-content:space-between;
align-items:flex-start;
gap:16px;
}
.course-title{
margin:0 0 6px;
font-weight:900;
font-size:1.35em;
line-height:1.25;
}
.course-meta{
color:#6b7280;
font-size:1.02em;
margin:0 0 14px;
}
.course-meta em{font-style:italic}

/* LEVEL BADGE like Published/Accepted */
.level-badge{
padding:8px 14px;
border-radius:999px;
font-weight:900;
font-size:.9em;
white-space:nowrap;
line-height:1;
margin-top:2px;
}
.level-grad{background:#dbeafe;color:#1e3a8a}        /* blue */
.level-undergrad{background:#dcfce7;color:#14532d}  /* green */

/* BUTTONS (one line, like research buttons) */
.course-actions{
display:flex;
flex-wrap:nowrap;
gap:14px;
margin:6px 0 0;
overflow-x:auto;
-webkit-overflow-scrolling:touch;
padding-bottom:2px;
}
.course-actions::-webkit-scrollbar{height:6px}
.course-actions::-webkit-scrollbar-thumb{background:#e5e7eb;border-radius:999px}
@media (min-width: 700px){
.course-actions{overflow-x:visible}
}
.action-btn{
display:inline-block;
padding:12px 18px;
border-radius:12px;
border:2px solid #b21619;
color:#b21619;
text-decoration:none !important;
font-weight:900;
font-size:1.05em;
transition:all .2s ease;
background:#fff;
white-space:nowrap;
flex:0 0 auto;
}
.action-btn:hover{background:#b21619;color:#fff}
.action-btn.blue{border-color:#3b82f6;color:#2563eb}
.action-btn.blue:hover{background:#3b82f6;color:#fff}

/* Summary panel */
.course-details{margin-top:14px}
.course-details .panel{
padding:14px 16px;
border:1px solid #e5e7eb;
border-radius:12px;
background:#fff;
}
.course-details .panel p{margin:0;color:#374151;line-height:1.65}
</style>

<div class="teaching-hero">
<h1>Teaching</h1>
<p>My teaching focuses on building strong analytical foundations in methods and political economy, combining hands-on data analysis, computational tools, and substantive theory to help students reason critically about politics, markets, and inequality.</p>
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
<div class="course-top">
<div>
<div class="course-title">POIR612 - Text as Data for Social Scientists 🤖</div>
<div class="course-meta">📍 <em>University of Southern California</em>, Fall 2025</div>
</div>
<span class="level-badge level-grad">Graduate</span>
</div>

<div class="course-actions">
<a class="action-btn" href="https://colab.research.google.com/drive/1YMkoWyMPIHYvRtw5RLlUnJ7wxDdVodfv?usp=sharing" target="_blank" rel="noopener">📄 Syllabus</a>
<a class="action-btn blue" href="https://www.notion.so/Text-as-Data-for-Social-Science-Classroom-Home-23510fb8267980cd8571c44bbae73eff?source=copy_link" target="_blank" rel="noopener">🌐 Course Website</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelector('.course-details').style.display = (this.closest('.course-box').querySelector('.course-details').style.display==='none'?'block':'none')">📖 Summary</a>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>The course introduces social scientists to computational techniques for analyzing large-scale textual information. Bridging NLP, machine learning, Bayesian statistics, and the social sciences, it emphasizes practical applications in political discourse analysis, sentiment detection, and policy communication. Students learn preprocessing, text representation (bag-of-words, embeddings), supervised learning, topic models, and modern transformer/LLM approaches, alongside ethical and methodological considerations.</p></div>
</div>
</div>
</article>

<!-- IR312 -->
<article class="course-card" data-level="undergrad" data-topics="methods">
<div class="course-box">
<div class="course-top">
<div>
<div class="course-title">IR312 - Intro to Data Analysis 📊</div>
<div class="course-meta">📍 <em>University of Southern California</em>, Spring 2026</div>
</div>
<span class="level-badge level-undergrad">Undergraduate</span>
</div>

<div class="course-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/Methods_Spring2026.pdf" target="_blank" rel="noopener">📄 Syllabus</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelector('.course-details').style.display = (this.closest('.course-box').querySelector('.course-details').style.display==='none'?'block':'none')">📖 Summary</a>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>How can we measure income inequality? What predicts election outcomes? Do policy interventions reduce poverty? This course equips students with tools to analyze data, draw statistical inferences, and apply causal reasoning to real-world political, social, and economic questions. No prior statistical background is required.</p></div>
</div>
</div>
</article>

<!-- IR430 -->
<article class="course-card" data-level="undergrad" data-topics="ipe">
<div class="course-box">
<div class="course-top">
<div>
<div class="course-title">IR430 - The Politics of International Trade 🌍</div>
<div class="course-meta">📍 <em>University of Southern California</em>, Spring 2026</div>
</div>
<span class="level-badge level-undergrad">Undergraduate</span>
</div>

<div class="course-actions">
<a class="action-btn" href="https://gonzalez-rostani.com/img/Papers/IPE_Spring2026.pdf" target="_blank" rel="noopener">📄 Syllabus</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelector('.course-details').style.display = (this.closest('.course-box').querySelector('.course-details').style.display==='none'?'block':'none')">📖 Summary</a>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>This course examines the political economy of international trade, connecting foundational theories and debates to contemporary issues. Students analyze how trade policies are made, who benefits and loses, and how global economic shifts shape domestic politics and international cooperation.</p></div>
</div>
</div>
</article>

<!-- MPE Quant Methods -->
<article class="course-card" data-level="undergrad" data-topics="methods ipe">
<div class="course-box">
<div class="course-top">
<div>
<div class="course-title">Mobilization and Political Economy, Quantitative Methods Course 📢</div>
<div class="course-meta">📍 <em>NSF-REU Summer Research Program</em>, Summer 2023</div>
</div>
<span class="level-badge level-undergrad">Undergraduate</span>
</div>

<div class="course-actions">
<a class="action-btn blue" href="https://www.migapprogram.com/" target="_blank" rel="noopener">🌐 MPE Website</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelectorAll('.course-details')[0].style.display = (this.closest('.course-box').querySelectorAll('.course-details')[0].style.display==='none'?'block':'none')">📖 Program summary</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelectorAll('.course-details')[1].style.display = (this.closest('.course-box').querySelectorAll('.course-details')[1].style.display==='none'?'block':'none')">📖 Course summary</a>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>The MPE Summer Program is an eight-week, in-residence research and mentoring initiative funded by NSF (REU Award #2150250). It supports underrepresented and first-generation undergraduates—especially from MSIs—through methodological training and structured guidance for graduate applications, connecting theory to hands-on data work.</p></div>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>The Quantitative Methods course builds a foundation in research design, descriptive statistics, and regression, then advances to hypothesis testing and multi-level modeling. Students learn R programming through real datasets (e.g., CMPS and census data), strengthening skills in data management, modeling, and applied policy analysis.</p></div>
</div>
</div>
</article>

<!-- PS0700 -->
<article class="course-card" data-level="undergrad" data-topics="methods">
<div class="course-box">
<div class="course-top">
<div>
<div class="course-title">PS0700 - Research Methods in Political Science ⚙️</div>
<div class="course-meta">📍 <em>University of Pittsburgh</em>, Summer 2022</div>
</div>
<span class="level-badge level-undergrad">Undergraduate</span>
</div>

<div class="course-actions">
<a class="action-btn" href="https://www.dropbox.com/s/shpfv8m1ke1iyr3/PS0700_S22.pdf?dl=0" target="_blank" rel="noopener">📄 Syllabus</a>
<a class="action-btn" href="javascript:void(0)" onclick="this.closest('.course-box').querySelector('.course-details').style.display = (this.closest('.course-box').querySelector('.course-details').style.display==='none'?'block':'none')">📖 Summary</a>
</div>

<div class="course-details" style="display:none">
<div class="panel"><p>This course builds students’ ability to understand and conduct quantitative political science research. Emphasis is on data analysis, inference, and causal reasoning, preparing students to interpret research methods used in academic work, policy memos, and social science reporting. No prior statistics required.</p></div>
</div>
</div>
</article>

# 🎤 Guest Lectures  

- _Mobilization and Political Economy_ NSF-REU Summer Camp: **The Political Economy of Automation**, Summer 2025.  
- _Political Economy of Growth_ (PS2543), University of Pittsburgh. **Technological Change and Automation of Jobs**, Spring 2023.  
- _Mobilization and Political Economy_ NSF-REU Summer Camp: **Theories of Political Economy**, Summer 2023.  

Slides available upon request. 

<br>
