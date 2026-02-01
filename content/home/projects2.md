+++
widget = "blank"
headless = true
active = true
weight = 60

title = "Research"
subtitle = ""

[design]
  columns = "1"

[design.spacing]
  padding = ["40px", "0", "40px", "0"]

[design.background]
  color = ""
  
[advanced]
 css_style = ""
 css_class = "research-page"
+++

{{< rawhtml >}}
<style>
@import url('https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600;700&family=Work+Sans:wght@400;500;600&display=swap');

.research-page {
  font-family: 'Work Sans', sans-serif;
}

.research-hero {
  text-align: center;
  margin-bottom: 60px;
  padding: 40px 20px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border-radius: 20px;
  color: white;
}

.research-hero h1 {
  font-family: 'Crimson Pro', serif;
  font-size: 3em;
  font-weight: 700;
  margin-bottom: 15px;
  color: white;
}

.research-hero p {
  font-size: 1.2em;
  opacity: 0.95;
  max-width: 800px;
  margin: 0 auto;
  line-height: 1.6;
}

.research-stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  margin-bottom: 50px;
}

.stat-card {
  background: white;
  padding: 25px;
  border-radius: 12px;
  text-align: center;
  border-left: 4px solid #667eea;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.stat-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}

.stat-number {
  font-size: 2.5em;
  font-weight: 700;
  color: #667eea;
  font-family: 'Crimson Pro', serif;
}

.stat-label {
  color: #6c757d;
  font-size: 0.95em;
  margin-top: 5px;
}

.themes-title {
  font-family: 'Crimson Pro', serif;
  font-size: 2em;
  font-weight: 600;
  margin: 50px 0 25px 0;
  color: #2d3748;
}

.theme-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 40px;
}

.theme-tag {
  padding: 10px 20px;
  border-radius: 25px;
  font-size: 0.95em;
  font-weight: 500;
  cursor: pointer;
  transition: all 0.3s ease;
  border: 2px solid transparent;
  color: white;
}

.theme-tag:hover {
  transform: scale(1.05);
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.theme-automation { background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); }
.theme-populism { background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); }
.theme-methods { background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%); }
.theme-latin-america { background: linear-gradient(135deg, #fa709a 0%, #fee140 100%); }
.theme-trade { background: linear-gradient(135deg, #30cfd0 0%, #330867 100%); }
.theme-all { background: #2d3748; }

.section-title {
  font-family: 'Crimson Pro', serif;
  font-size: 2em;
  font-weight: 600;
  margin: 60px 0 30px 0;
  color: #2d3748;
  border-bottom: 3px solid #667eea;
  padding-bottom: 10px;
  display: inline-block;
}

.featured-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 30px;
  margin-bottom: 50px;
}

.featured-card {
  background: white;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 1px solid #e2e8f0;
}

.featured-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 40px rgba(0,0,0,0.15);
}

.featured-header {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  padding: 30px;
  color: white;
}

.featured-title {
  font-family: 'Crimson Pro', serif;
  font-size: 1.4em;
  font-weight: 600;
  margin-bottom: 10px;
  line-height: 1.3;
  color: white;
}

.featured-journal {
  font-size: 0.9em;
  opacity: 0.9;
  font-style: italic;
}

.featured-body {
  padding: 25px;
}

.featured-abstract {
  color: #4a5568;
  line-height: 1.7;
  margin-bottom: 20px;
  font-size: 0.95em;
}

.featured-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 15px;
}

.mini-tag {
  padding: 4px 12px;
  border-radius: 15px;
  font-size: 0.8em;
  font-weight: 500;
  color: white;
}

.featured-links {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}

.paper-link {
  padding: 8px 16px;
  border-radius: 8px;
  text-decoration: none;
  font-size: 0.9em;
  font-weight: 500;
  transition: all 0.3s ease;
  display: inline-block;
  background: #667eea;
  color: white;
}

.paper-link:hover {
  background: #5568d3;
  transform: translateY(-2px);
  color: white;
  text-decoration: none;
}

.filter-controls {
  display: flex;
  gap: 15px;
  margin-bottom: 30px;
  flex-wrap: wrap;
  align-items: center;
}

.filter-label {
  font-weight: 600;
  color: #2d3748;
}

.status-filter {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}

.status-btn {
  padding: 8px 18px;
  border-radius: 20px;
  border: 2px solid #e2e8f0;
  background: white;
  cursor: pointer;
  font-size: 0.9em;
  font-weight: 500;
  transition: all 0.3s ease;
}

.status-btn:hover {
  border-color: #667eea;
}

.status-btn.active {
  background: #667eea;
  color: white;
  border-color: #667eea;
}

.pub-card {
  background: white;
  border-radius: 12px;
  padding: 25px;
  border-left: 5px solid #e2e8f0;
  transition: all 0.3s ease;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  margin-bottom: 20px;
}

.pub-card:hover {
  border-left-color: #667eea;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  transform: translateX(5px);
}

.pub-card.hidden {
  display: none;
}

.pub-header {
  display: flex;
  justify-content: space-between;
  align-items: start;
  margin-bottom: 15px;
  gap: 15px;
}

.pub-title-block {
  flex: 1;
}

.pub-title {
  font-family: 'Crimson Pro', serif;
  font-size: 1.3em;
  font-weight: 600;
  color: #2d3748;
  margin-bottom: 8px;
  line-height: 1.4;
}

.pub-title a {
  color: #2d3748;
  text-decoration: none;
  transition: color 0.3s ease;
}

.pub-title a:hover {
  color: #667eea;
}

.pub-authors {
  color: #718096;
  font-size: 0.95em;
  margin-bottom: 5px;
}

.pub-venue {
  color: #4a5568;
  font-style: italic;
  font-size: 0.95em;
}

.pub-status {
  padding: 6px 14px;
  border-radius: 15px;
  font-size: 0.85em;
  font-weight: 500;
  white-space: nowrap;
}

.status-published { background: #c6f6d5; color: #22543d; }
.status-forthcoming { background: #bee3f8; color: #2c5282; }
.status-under-review { background: #feebc8; color: #7c2d12; }
.status-working { background: #e2e8f0; color: #2d3748; }

.pub-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 15px;
}

@media (max-width: 768px) {
  .research-hero h1 { font-size: 2em; }
  .featured-grid { grid-template-columns: 1fr; }
  .filter-controls { flex-direction: column; align-items: flex-start; }
  .pub-header { flex-direction: column; }
}
</style>

<div class="research-hero">
  <h1>Research Portfolio</h1>
  <p>Exploring how technological change—especially automation and artificial intelligence—reshapes politics, labor markets, and democratic institutions across advanced and developing economies.</p>
</div>

<div class="research-stats">
  <div class="stat-card">
    <div class="stat-number">8</div>
    <div class="stat-label">Published Articles</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">5</div>
    <div class="stat-label">Under Review</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">10+</div>
    <div class="stat-label">Working Papers</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">4</div>
    <div class="stat-label">Research Themes</div>
  </div>
</div>

<h2 class="themes-title">Research Themes</h2>
<div class="theme-tags">
  <div class="theme-tag theme-all">All Research</div>
  <div class="theme-tag theme-automation">🤖 Automation & AI Politics</div>
  <div class="theme-tag theme-populism">🗳️ Populism & Polarization</div>
  <div class="theme-tag theme-methods">📊 Political Methodology</div>
  <div class="theme-tag theme-latin-america">🌎 Latin American Politics</div>
  <div class="theme-tag theme-trade">🏭 Trade & Labor</div>
</div>

<h2 class="section-title">Featured Research</h2>
<div class="featured-grid">
  
  <div class="featured-card">
    <div class="featured-header">
      <div class="featured-title">Elections, Right-wing Populism, and Political-Economic Polarization</div>
      <div class="featured-journal">The Journal of Politics (2026)</div>
    </div>
    <div class="featured-body">
      <div class="featured-abstract">
        How have right-wing populists attracted routine workers previously loyal to mainstream left-wing parties? This project builds a theoretical model explaining populist success across majoritarian and proportional systems, using vote-switching data and AI-analyzed campaign rhetoric from the US and Germany.
      </div>
      <div class="featured-tags">
        <span class="mini-tag theme-automation">Automation</span>
        <span class="mini-tag theme-populism">Populism</span>
        <span class="mini-tag theme-methods">Text-as-Data</span>
      </div>
      <div class="featured-links">
        <a href="https://www.journals.uchicago.edu/doi/10.1086/734533" class="paper-link" target="_blank">Read Paper</a>
        <a href="https://gonzalez-rostani.com/img/Papers/Revised_ms.pdf" class="paper-link" target="_blank">Pre-Print</a>
      </div>
    </div>
  </div>

  <div class="featured-card">
    <div class="featured-header">
      <div class="featured-title">Engaged Robots, Disengaged Workers: Automation and Political Apathy</div>
      <div class="featured-journal">Economics & Politics (2024)</div>
    </div>
    <div class="featured-body">
      <div class="featured-abstract">
        Using 23 European countries' data (2002-2018), I show that workers exposed to automation are 10% less likely to be politically engaged. Income and unionization moderate this effect, revealing how economic inequality and automation reinforce political disengagement.
      </div>
      <div class="featured-tags">
        <span class="mini-tag theme-automation">Automation</span>
        <span class="mini-tag theme-populism">Political Behavior</span>
      </div>
      <div class="featured-links">
        <a href="http://doi.org/10.1111/ecpo.12307" class="paper-link" target="_blank">Read Paper</a>
      </div>
    </div>
  </div>

  <div class="featured-card">
    <div class="featured-header">
      <div class="featured-title">The Political Economy of Automation in Global Value Chains</div>
      <div class="featured-journal">With Carles Boix & Erica Owen</div>
    </div>
    <div class="featured-body">
      <div class="featured-abstract">
        How does automation in advanced economies affect politics in developing countries? Using Mexican data, we show robot adoption in the US reduces export-oriented employment, increasing violence and left-populist support. Automation shocks ripple through global value chains.
      </div>
      <div class="featured-tags">
        <span class="mini-tag theme-automation">Automation</span>
        <span class="mini-tag theme-trade">Global Trade</span>
        <span class="mini-tag theme-latin-america">Latin America</span>
      </div>
      <div class="featured-links">
        <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058" class="paper-link" target="_blank">Working Paper</a>
      </div>
    </div>
  </div>

</div>

<h2 class="section-title">All Publications</h2>

<div class="filter-controls">
  <span class="filter-label">Filter by status:</span>
  <div class="status-filter">
    <button class="status-btn active" onclick="filterStatus('all')">All</button>
    <button class="status-btn" onclick="filterStatus('published')">Published</button>
    <button class="status-btn" onclick="filterStatus('under-review')">Under Review</button>
    <button class="status-btn" onclick="filterStatus('working')">Working Papers</button>
  </div>
</div>

<div id="publications-grid">
  
  <div class="pub-card" data-status="published">
    <div class="pub-header">
      <div class="pub-title-block">
        <div class="pub-title">
          <a href="https://www.journals.uchicago.edu/doi/10.1086/734533" target="_blank">Elections, Right-wing Populism, and Political-Economic Polarization</a>
        </div>
        <div class="pub-authors">Valentina González-Rostani</div>
        <div class="pub-venue">The Journal of Politics, Vol. 88, No. 1 (2026)</div>
      </div>
      <div class="pub-status status-published">Published</div>
    </div>
    <div class="pub-tags">
      <span class="mini-tag theme-populism">Populism</span>
      <span class="mini-tag theme-automation">Automation</span>
    </div>
  </div>

  <div class="pub-card" data-status="published">
    <div class="pub-header">
      <div class="pub-title-block">
        <div class="pub-title">
          <a href="http://doi.org/10.1111/ecpo.12307" target="_blank">Engaged Robots, and Disengaged Workers: Automation and Political Apathy</a>
        </div>
        <div class="pub-authors">Valentina González-Rostani</div>
        <div class="pub-venue">Economics & Politics (2024)</div>
      </div>
      <div class="pub-status status-published">Published</div>
    </div>
    <div class="pub-tags">
      <span class="mini-tag theme-automation">Automation</span>
    </div>
  </div>

  <div class="pub-card" data-status="published">
    <div class="pub-header">
      <div class="pub-title-block">
        <div class="pub-title">
          <a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481" target="_blank">Social Media versus Surveys: A New Scalable Approach</a>
        </div>
        <div class="pub-authors">with Jose Luis Incio and Guillermo Lezama</div>
        <div class="pub-venue">Legislative Studies Quarterly (2024)</div>
      </div>
      <div class="pub-status status-published">Published</div>
    </div>
    <div class="pub-tags">
      <span class="mini-tag theme-methods">Text-as-Data</span>
      <span class="mini-tag theme-latin-america">Latin America</span>
    </div>
  </div>

  <div class="pub-card" data-status="under-review">
    <div class="pub-header">
      <div class="pub-title-block">
        <div class="pub-title">The Path from Automation to Right-Wing Populism</div>
        <div class="pub-authors">Valentina González-Rostani</div>
        <div class="pub-venue">Under Review</div>
      </div>
      <div class="pub-status status-under-review">Under Review</div>
    </div>
    <div class="pub-tags">
      <span class="mini-tag theme-automation">Automation</span>
      <span class="mini-tag theme-populism">Populism</span>
    </div>
  </div>

  <div class="pub-card" data-status="working">
    <div class="pub-header">
      <div class="pub-title-block">
        <div class="pub-title">
          <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058" target="_blank">The Political Economy of Automation and Fragmented Production: Evidence from Mexico</a>
        </div>
        <div class="pub-authors">with Carles Boix and Erica Owen</div>
        <div class="pub-venue">Working Paper</div>
      </div>
      <div class="pub-status status-working">Working Paper</div>
    </div>
    <div class="pub-tags">
      <span class="mini-tag theme-automation">Automation</span>
      <span class="mini-tag theme-trade">Trade</span>
      <span class="mini-tag theme-latin-america">Latin America</span>
    </div>
  </div>

</div>

<script>
function filterStatus(status) {
  const cards = document.querySelectorAll('.pub-card');
  const buttons = document.querySelectorAll('.status-btn');
  
  buttons.forEach(btn => btn.classList.remove('active'));
  event.target.classList.add('active');
  
  cards.forEach(card => {
    if (status === 'all' || card.dataset.status === status) {
      card.classList.remove('hidden');
    } else {
      card.classList.add('hidden');
    }
  });
}
</script>

{{< /rawhtml >}}
