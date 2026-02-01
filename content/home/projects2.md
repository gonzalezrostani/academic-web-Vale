+++
widget = "blank"
headless = true
active = true
weight = 60  # Adjust based on where you want it in your page order

title = "Research"
subtitle = ""

[design]
  columns = "1"

[design.spacing]
  padding = ["40px", "0", "40px", "0"]
+++

<style>
@import url('https://fonts.googleapis.com/css2?family=Crimson+Pro:wght@400;600;700&family=Work+Sans:wght@400;500;600&display=swap');

.research-container {
  max-width: 1400px;
  margin: 0 auto;
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
  background: #f8f9fa;
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

.research-themes {
  margin-bottom: 50px;
}

.themes-title {
  font-family: 'Crimson Pro', serif;
  font-size: 2em;
  font-weight: 600;
  margin-bottom: 25px;
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
}

.theme-tag.active {
  transform: scale(1.05);
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.theme-automation {
  background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
  color: white;
}

.theme-automation.active {
  border-color: #f5576c;
}

.theme-populism {
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
  color: white;
}

.theme-populism.active {
  border-color: #00f2fe;
}

.theme-methods {
  background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
  color: white;
}

.theme-methods.active {
  border-color: #38f9d7;
}

.theme-latin-america {
  background: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
  color: white;
}

.theme-latin-america.active {
  border-color: #fee140;
}

.theme-trade {
  background: linear-gradient(135deg, #30cfd0 0%, #330867 100%);
  color: white;
}

.theme-trade.active {
  border-color: #330867;
}

.theme-all {
  background: #2d3748;
  color: white;
}

.theme-all.active {
  background: #1a202c;
  border-color: #667eea;
}

/* FEATURED PROJECTS */
.featured-section {
  margin-bottom: 60px;
}

.section-title {
  font-family: 'Crimson Pro', serif;
  font-size: 2em;
  font-weight: 600;
  margin-bottom: 30px;
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
}

.link-paper {
  background: #667eea;
  color: white;
}

.link-paper:hover {
  background: #5568d3;
  transform: translateY(-2px);
}

.link-code {
  background: #48bb78;
  color: white;
}

.link-code:hover {
  background: #38a169;
  transform: translateY(-2px);
}

.publications-section {
  margin-top: 60px;
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

.publications-grid {
  display: grid;
  gap: 20px;
}

.pub-card {
  background: white;
  border-radius: 12px;
  padding: 25px;
  border-left: 5px solid #e2e8f0;
  transition: all 0.3s ease;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
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

.status-published {
  background: #c6f6d5;
  color: #22543d;
}

.status-forthcoming {
  background: #bee3f8;
  color: #2c5282;
}

.status-under-review {
  background: #feebc8;
  color: #7c2d12;
}

.status-working {
  background: #e2e8f0;
  color: #2d3748;
}

.pub-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 15px;
}

@media (max-width: 768px) {
  .research-hero h1 {
    font-size: 2em;
  }
  
  .featured-grid {
    grid-template-columns: 1fr;
  }
  
  .filter-controls {
    flex-direction: column;
    align-items: flex-start;
  }
  
  .pub-header {
    flex-direction: column;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.pub-card {
  animation: fadeIn 0.5s ease forwards;
}

</style>

<div class="research-container">

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

<div class="research-themes">
  <h2 class="themes-title">Research Themes</h2>
  <div class="theme-tags">
    <div class="theme-tag theme-all active" onclick="filterByTheme('all')">
      All Research
    </div>
    <div class="theme-tag theme-automation" onclick="filterByTheme('automation')">
      🤖 Automation & AI Politics
    </div>
    <div class="theme-tag theme-populism" onclick="filterByTheme('populism')">
      🗳️ Populism & Polarization
    </div>
    <div class="theme-tag theme-methods" onclick="filterByTheme('methods')">
      📊 Political Methodology
    </div>
    <div class="theme-tag theme-latin-america" onclick="filterByTheme('latin-america')">
      🌎 Latin American Politics
    </div>
    <div class="theme-tag theme-trade" onclick="filterByTheme('trade')">
      🏭 Trade & Labor
    </div>
  </div>
</div>

<div class="featured-section">
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
          <a href="https://www.journals.uchicago.edu/doi/10.1086/734533" class="paper-link link-paper" target="_blank">Read Paper</a>
          <a href="https://gonzalez-rostani.com/img/Papers/Revised_ms.pdf" class="paper-link link-paper" target="_blank">Pre-Print</a>
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
          <a href="http://doi.org/10.1111/ecpo.12307" class="paper-link link-paper" target="_blank">Read Paper</a>
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
          <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5553058" class="paper-link link-paper" target="_blank">Working Paper</a>
        </div>
      </div>
    </div>

  </div>
</div>

<div class="publications-section">
  <h2 class="section-title">All Publications</h2>
  
  <div class="filter-controls">
    <span class="filter-label">Filter by status:</span>
    <div class="status-filter">
      <button class="status-btn active" onclick="filterByStatus('all')">All</button>
      <button class="status-btn" onclick="filterByStatus('published')">Published</button>
      <button class="status-btn" onclick="filterByStatus('under-review')">Under Review</button>
      <button class="status-btn" onclick="filterByStatus('working')">Working Papers</button>
    </div>
  </div>

  <div class="publications-grid" id="publications-grid">
    
    <div class="pub-card" data-status="published" data-themes="populism automation methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://www.journals.uchicago.edu/doi/10.1086/734533" target="_blank">Elections, Right-wing Populism, and Political-Economic Polarization: The Role of Institutions and Political Outsiders</a>
          </div>
          <div class="pub-authors">Valentina González-Rostani</div>
          <div class="pub-venue">The Journal of Politics, Vol. 88, No. 1 (2026)</div>
        </div>
        <div class="pub-status status-published">Published</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-populism">Populism</span>
        <span class="mini-tag theme-automation">Automation</span>
        <span class="mini-tag theme-methods">Text-as-Data</span>
      </div>
    </div>

    <div class="pub-card" data-status="forthcoming" data-themes="trade methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf" target="_blank">Love of Variety? An Experimental Study of Heterogeneous Responses to Foreign Brands in the Marketplace</a>
          </div>
          <div class="pub-authors">with Jude C. Hays</div>
          <div class="pub-venue">Political Science Research and Methods (2026)</div>
        </div>
        <div class="pub-status status-forthcoming">Conditionally Accepted</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-trade">Trade</span>
        <span class="mini-tag theme-methods">Experiments</span>
      </div>
    </div>

    <div class="pub-card" data-status="published" data-themes="methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://cup.org/4ibfZqa" target="_blank">Engaging Diversity: An Inclusive Approach to Undergraduate Mentorship in Mobilization and Political Economy</a>
          </div>
          <div class="pub-authors">with Chie Togami, Mariely Lopez-Santana, Tania Ramirez, Fernando Tormos-Aponte, and Mayra Velez-Serrano</div>
          <div class="pub-venue">PS: Political Science & Politics (2025)</div>
        </div>
        <div class="pub-status status-published">Published</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-methods">Methods</span>
      </div>
    </div>

    <div class="pub-card" data-status="published" data-themes="populism methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://www.tandfonline.com/doi/abs/10.1080/17457289.2025.2504860" target="_blank">Are Protests Contagious? The Dynamics of Temporal and Spatial Diffusion of Political Protests</a>
          </div>
          <div class="pub-authors">with Jeffrey Nonnemacher</div>
          <div class="pub-venue">Journal of Elections, Public Opinion & Parties (2025)</div>
        </div>
        <div class="pub-status status-published">Published</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-populism">Political Behavior</span>
        <span class="mini-tag theme-methods">Spatial Methods</span>
      </div>
    </div>

    <div class="pub-card" data-status="published" data-themes="automation">
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
        <span class="mini-tag theme-populism">Political Behavior</span>
      </div>
    </div>

    <div class="pub-card" data-status="published" data-themes="methods latin-america">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481" target="_blank">Social Media versus Surveys: A New Scalable Approach to Understanding Political Discourse</a>
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

    <div class="pub-card" data-status="published" data-themes="latin-america">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476" target="_blank">How Germane are Moral and Economic Policies to Ideology? Evidence from Latin American Legislators</a>
          </div>
          <div class="pub-authors">with Elias Chavarria, Chuang Chen, and Scott Morgenstern</div>
          <div class="pub-venue">Legislative Studies Quarterly (2024)</div>
        </div>
        <div class="pub-status status-published">Published</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-latin-america">Latin America</span>
      </div>
    </div>

    <div class="pub-card" data-status="published" data-themes="latin-america">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://www.cambridge.org/core/journals/latin-american-research-review/article/legislators-religiosity-and-samesex-marriage-in-latin-america/E1036194383293859C18F10394554923" target="_blank">Legislators' Religiosity and Same-Sex Marriage in Latin America</a>
          </div>
          <div class="pub-authors">with Scott Morgenstern</div>
          <div class="pub-venue">Latin American Research Review (2023)</div>
        </div>
        <div class="pub-status status-published">Published</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-latin-america">Latin America</span>
      </div>
    </div>

    <div class="pub-card" data-status="under-review" data-themes="automation">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">The Threat of Automation and Public Support for Environmental Regulation</div>
          <div class="pub-authors">with Michaël Aklin and Liam Beiser-McGrath</div>
          <div class="pub-venue">R&R at Ecological Economics</div>
        </div>
        <div class="pub-status status-under-review">Under Review</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-automation">Automation</span>
      </div>
    </div>

    <div class="pub-card" data-status="under-review" data-themes="automation populism">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://gonzalez-rostani.com/img/Papers/APSA_Automation_Culture.pdf" target="_blank">The Path from Automation to Right-Wing Populism</a>
          </div>
          <div class="pub-authors">Valentina González-Rostani</div>
          <div class="pub-venue">Under Review</div>
        </div>
        <div class="pub-status status-under-review">Under Review</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-automation">Automation</span>
        <span class="mini-tag theme-populism">Populism</span>
        <span class="mini-tag theme-methods">Experiments</span>
      </div>
    </div>

    <div class="pub-card" data-status="under-review" data-themes="automation methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://gonzalez-rostani.com/img/Papers/Subjective_Techrisk.pdf" target="_blank">Navigating Uncertainty: How Experience Shapes Perception and Politics in the AI Era</a>
          </div>
          <div class="pub-authors">with Tobias Tober</div>
          <div class="pub-venue">Under Review</div>
        </div>
        <div class="pub-status status-under-review">Under Review</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-automation">AI</span>
        <span class="mini-tag theme-methods">Survey Research</span>
      </div>
    </div>

    <div class="pub-card" data-status="under-review" data-themes="latin-america methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">
            <a href="https://gonzalez-rostani.com/img/Papers/Immigration.pdf" target="_blank">Immigration Shocks and Politicians' Rhetoric: Evidence from The Venezuelan Migration Crisis</a>
          </div>
          <div class="pub-authors">with Jose Luis Incio and Guillermo Lezama</div>
          <div class="pub-venue">Under Review</div>
        </div>
        <div class="pub-status status-under-review">Under Review</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-latin-america">Latin America</span>
        <span class="mini-tag theme-methods">Text-as-Data</span>
      </div>
    </div>

    <div class="pub-card" data-status="working" data-themes="automation trade latin-america">
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
        <span class="mini-tag theme-trade">Global Trade</span>
        <span class="mini-tag theme-latin-america">Latin America</span>
      </div>
    </div>

    <div class="pub-card" data-status="working" data-themes="populism methods">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">Who Influences Whom? Analyzing the Interplay of Mainstream and Outsider Parties in Social Media Campaigns</div>
          <div class="pub-authors">Valentina González-Rostani</div>
          <div class="pub-venue">Working Paper</div>
        </div>
        <div class="pub-status status-working">Working Paper</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-populism">Populism</span>
        <span class="mini-tag theme-methods">Text-as-Data</span>
      </div>
    </div>

    <div class="pub-card" data-status="working" data-themes="methods populism">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">You Can't Stop It If You Can't See It: Introducing a New Scalable System to Measure Populist Narratives at Higher Resolution</div>
          <div class="pub-authors">with Bree Bang-Jensen and Michael Colaresi</div>
          <div class="pub-venue">Working Paper</div>
        </div>
        <div class="pub-status status-working">Working Paper</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-methods">NLP</span>
        <span class="mini-tag theme-populism">Populism</span>
      </div>
    </div>

    <div class="pub-card" data-status="working" data-themes="automation">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">Augmentation or Displacement? The Behavioral and Policy Implications of AI-Assisted Work</div>
          <div class="pub-authors">with Shir Raviv</div>
          <div class="pub-venue">Working Paper</div>
        </div>
        <div class="pub-status status-working">Working Paper</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-automation">AI</span>
        <span class="mini-tag theme-methods">Experiments</span>
      </div>
    </div>

    <div class="pub-card" data-status="working" data-themes="automation">
      <div class="pub-header">
        <div class="pub-title-block">
          <div class="pub-title">Artificial Intelligence and the Future of Democracy: Political and Institutional Consequences of Economic Dislocation</div>
          <div class="pub-authors">with Carles Boix</div>
          <div class="pub-venue">Working Paper</div>
        </div>
        <div class="pub-status status-working">Working Paper</div>
      </div>
      <div class="pub-tags">
        <span class="mini-tag theme-automation">AI</span>
      </div>
    </div>

  </div>
</div>

</div>

<script>
let currentTheme = 'all';
let currentStatus = 'all';

function filterByTheme(theme) {
  currentTheme = theme;
  applyFilters();
  
  document.querySelectorAll('.theme-tag').forEach(tag => {
    tag.classList.remove('active');
  });
  event.target.classList.add('active');
}

function filterByStatus(status) {
  currentStatus = status;
  applyFilters();
  
  document.querySelectorAll('.status-btn').forEach(btn => {
    btn.classList.remove('active');
  });
  event.target.classList.add('active');
}

function applyFilters() {
  const cards = document.querySelectorAll('.pub-card');
  
  cards.forEach(card => {
    const cardStatus = card.dataset.status;
    const cardThemes = card.dataset.themes ? card.dataset.themes.split(' ') : [];
    
    let showCard = true;
    
    if (currentStatus !== 'all' && cardStatus !== currentStatus) {
      showCard = false;
    }
    
    if (currentTheme !== 'all' && !cardThemes.includes(currentTheme)) {
      showCard = false;
    }
    
    if (showCard) {
      card.classList.remove('hidden');
    } else {
      card.classList.add('hidden');
    }
  });
}
</script>
