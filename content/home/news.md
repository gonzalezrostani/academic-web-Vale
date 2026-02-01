+++
# A Demo section created with the Blank widget.
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 45  # Order that this section will appear - adjust based on your other sections

title = "News & Events"
subtitle = ""

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"
  
  # Background image.
  # image = "background.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.

  # Text color (true=light or false=dark).
  # text_color_light = true

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

<style>
.news-section {
  max-width: 1200px;
  margin: 0 auto;
}

.news-table {
  width: 100%;
  border-collapse: collapse;
  margin: 20px 0;
  font-size: 0.95em;
}

.news-table th {
  background-color: #f8f9fa;
  padding: 12px 15px;
  text-align: left;
  font-weight: 600;
  border-bottom: 2px solid #dee2e6;
  color: #495057;
}

.news-table td {
  padding: 10px 15px;
  border-bottom: 1px solid #e9ecef;
  vertical-align: top;
}

.news-table tr:hover {
  background-color: #f8f9fa;
}

.event-type {
  display: inline-block;
  padding: 2px 8px;
  border-radius: 3px;
  font-size: 0.85em;
  font-weight: 500;
}

.type-publication {
  background-color: #d1ecf1;
  color: #0c5460;
}

.type-talk {
  background-color: #d4edda;
  color: #155724;
}

.type-panel {
  background-color: #fff3cd;
  color: #856404;
}

.type-award {
  background-color: #f8d7da;
  color: #721c24;
}

.type-participant {
  background-color: #e2e3e5;
  color: #383d41;
}

.type-workshop {
  background-color: #cfe2ff;
  color: #084298;
}

.scheduled-tag {
  font-style: italic;
  color: #6c757d;
  font-size: 0.9em;
}

.year-section {
  margin: 30px 0;
}

.year-header {
  font-size: 1.5em;
  font-weight: 600;
  margin-bottom: 15px;
  padding-bottom: 10px;
  border-bottom: 2px solid #007bff;
  color: #333;
  cursor: pointer;
  user-select: none;
  display: flex;
  align-items: center;
}

.year-header:hover {
  color: #007bff;
}

.toggle-icon {
  margin-left: 10px;
  font-size: 0.8em;
  transition: transform 0.3s ease;
}

.toggle-icon.collapsed {
  transform: rotate(-90deg);
}

.year-content {
  overflow: hidden;
  transition: max-height 0.3s ease;
}

.year-content.collapsed {
  max-height: 0;
}

.year-content.expanded {
  max-height: 5000px;
}

.news-intro {
  margin-bottom: 30px;
  color: #6c757d;
}

@media (max-width: 768px) {
  .news-table {
    font-size: 0.85em;
  }
  
  .news-table th,
  .news-table td {
    padding: 8px 10px;
  }
  
  .year-header {
    font-size: 1.3em;
  }
}
</style>

<div class="news-section">

<div class="year-section">
  <div class="year-header" onclick="toggleYear('2026')">
    📅 2026 News
    <span class="toggle-icon" id="icon-2026">▼</span>
  </div>
  <div class="year-content expanded" id="content-2026">
    <table class="news-table">
      <thead>
        <tr>
          <th style="width: 12%;">Date</th>
          <th style="width: 15%;">Type</th>
          <th style="width: 48%;">Event</th>
          <th style="width: 25%;">Place</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Spring 2026</td>
          <td><span class="event-type type-talk">Teaching</span></td>
          <td>The Politics of International Trade (Undergraduate)</td>
          <td>USC</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Texas A&M University - Globalization Backlash: New Theory and Evidence <span class="scheduled-tag">(upcoming)</span></td>
          <td>Texas A&M</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>University of California, Riverside <span class="scheduled-tag">(upcoming)</span></td>
          <td>UC Riverside</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>University of Washington - Severyns-Ravenholt Seminar in Comparative Politics <span class="scheduled-tag">(upcoming)</span></td>
          <td>Seattle, WA</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>USC Center for International Studies - IR Seminar <span class="scheduled-tag">(upcoming)</span></td>
          <td>Los Angeles, CA</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>USC Sol Price School - Political Institutions and Political Economy Seminar <span class="scheduled-tag">(upcoming)</span></td>
          <td>Los Angeles, CA</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-workshop">Workshop</span></td>
          <td>APSA Labor Politics Group Virtual Workshop <span class="scheduled-tag">(upcoming)</span></td>
          <td>Virtual</td>
        </tr>
        <tr>
          <td>2026</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://gonzalez-rostani.com/img/Papers/LoV_updated.pdf">Love of Variety? Experimental Study of Foreign Brands</a> (with Jude Hays) - <i>Political Science Research and Methods</i> <span class="scheduled-tag">(conditionally accepted)</span></td>
          <td>Forthcoming</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="year-section">
  <div class="year-header" onclick="toggleYear('2025')">
    📅 2025 News
    <span class="toggle-icon collapsed" id="icon-2025">▼</span>
  </div>
  <div class="year-content collapsed" id="content-2025">
    <table class="news-table">
      <thead>
        <tr>
          <th style="width: 12%;">Date</th>
          <th style="width: 15%;">Type</th>
          <th style="width: 48%;">Event</th>
          <th style="width: 25%;">Place</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Fall 2025</td>
          <td><span class="event-type type-award">Position</span></td>
          <td>Started as Assistant Professor at USC</td>
          <td>Los Angeles, CA</td>
        </tr>
        <tr>
          <td>Fall 2025</td>
          <td><span class="event-type type-talk">Teaching</span></td>
          <td>Advanced Methodology: Text as Data (Graduate)</td>
          <td>USC</td>
        </tr>
        <tr>
          <td>Spring 2025</td>
          <td><span class="event-type type-talk">Teaching</span></td>
          <td>Introduction to Data Analysis (Undergraduate)</td>
          <td>USC</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-award">Award</span></td>
          <td>Appointed to National System of Researchers (SNI), ANII, Uruguay</td>
          <td>Uruguay</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-award">Award</span></td>
          <td>Member of APSA Task Force on AI and Political Science - Economic Inequality and Labor Force Committee</td>
          <td>APSA</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-award">Grant</span></td>
          <td>Center for International Studies Research Award - $10,000</td>
          <td>Princeton University</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-award">Grant</span></td>
          <td>Invited to submit full proposal following LOI - Russell Sage Foundation - $200,000</td>
          <td>RSF</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-workshop">Training</span></td>
          <td>Gen AI Intensive Course with Google - Prompt engineering, embeddings, and generative AI agents</td>
          <td>Google</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Speaker</span></td>
          <td>WS x Columbia University - The Return of Donald Trump: Implications for US-China Relations Fireside Talk Series</td>
          <td>Columbia University</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://www.journals.uchicago.edu/doi/10.1086/734533">Elections, Right-wing Populism, and Political-Economic Polarization</a> - <i>The Journal of Politics</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://cup.org/4ibfZqa">Engaging Diversity: Inclusive Approach to Undergraduate Mentorship</a> (with Togami et al.) - <i>PS: Political Science & Politics</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td>Are Protests Contagious? Temporal and Spatial Diffusion (with Jeffrey Nonnemacher) - <i>Journal of Elections, Public Opinion & Parties</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Chair</span></td>
          <td>APPAM Panel Chair</td>
          <td>APPAM Conference</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Columbia University</td>
          <td>New York, NY</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Inter-American Development Bank - Digital Technologies, Growth & Well-Being in Emerging Economies</td>
          <td>IDB</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-workshop">Workshop</span></td>
          <td>Monash–Paris–Warwick–Zurich–CEPR - 10th Text-As-Data Workshop</td>
          <td>International</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>MPE-NSF REU - Mobilization and Political Economy</td>
          <td>University of Pittsburgh</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>NYU - Data Science Frontiers: Society and Politics</td>
          <td>New York, NY</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Penn State–Pitt IR Annual Workshop</td>
          <td>PA</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-workshop">Workshop</span></td>
          <td>Special Issue Workshop "The Future of Labor"</td>
          <td>International</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>IBEIC Institut Barcelona - The Politics of AI: Actors, Policy, Geopolitics, and Resistances</td>
          <td>Barcelona, Spain</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>University of Nebraska–Lincoln - Hendricks Symposium: Bordering on Crisis?</td>
          <td>Lincoln, NE</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>University of Pennsylvania - Junior Scholars in International Relations</td>
          <td>Philadelphia, PA</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Universidad de la Republica - DECON & DCPU</td>
          <td>Montevideo, Uruguay</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Yale University ISPS - AI and Governance</td>
          <td>New Haven, CT</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>APPAM (Association for Public Policy Analysis and Management)</td>
          <td>Conference</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>IPES (International Political Economy Society)</td>
          <td>Conference</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>ISA (International Studies Association)</td>
          <td>Conference</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>MPSA (Midwest Political Science Association)</td>
          <td>Chicago, IL</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>PolMeth (Political Methodology)</td>
          <td>Conference</td>
        </tr>
        <tr>
          <td>2025</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>EPSA (European Political Science Association)</td>
          <td>Conference</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="year-section">
  <div class="year-header" onclick="toggleYear('2024')">
    📅 2024 News
    <span class="toggle-icon collapsed" id="icon-2024">▼</span>
  </div>
  <div class="year-content collapsed" id="content-2024">
    <table class="news-table">
      <thead>
        <tr>
          <th style="width: 12%;">Date</th>
          <th style="width: 15%;">Type</th>
          <th style="width: 48%;">Event</th>
          <th style="width: 25%;">Place</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-award">Position</span></td>
          <td>Began Postdoctoral Research Associate position at Princeton University (supervised by Carles Boix)</td>
          <td>Princeton, NJ</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-award">Award</span></td>
          <td>Completed Ph.D. in Political Science</td>
          <td>University of Pittsburgh</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-award">Position</span></td>
          <td>Co-director of social science blog Razones y Personas</td>
          <td>Online</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="http://doi.org/10.1111/ecpo.12307">Engaged Robots, and Disengaged Workers: Automation and Political Apathy</a> - <i>Economics & Politics</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481">Social Media vs. Surveys: New Scalable Approach</a> (with Incio & Lezama) - <i>Legislative Studies Quarterly</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476">Moral and Economic Dimensions of Ideology</a> (with Morgenstern et al.) - <i>Legislative Studies Quarterly</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Caltech CSSPP - Navigating the New Frontier: Political and Economic Implications of AI Conference</td>
          <td>Pasadena, CA</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Princeton University - Niehaus Center, IR Faculty Colloquium</td>
          <td>Princeton, NJ</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Princeton University - Political Economy Colloquium</td>
          <td>Princeton, NJ</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Yale University MacMillan Center - New Challenges for International Cooperation: Automation, AI and Digital Trade</td>
          <td>New Haven, CT</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>APSA (American Political Science Association)</td>
          <td>Philadelphia, PA</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>IPES (International Political Economy Society) - Virtual</td>
          <td>Virtual</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>LACEA-LAMES (Latin American and Caribbean Economic Association)</td>
          <td>Conference</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>LAPolMeth (Latin American Political Methodology)</td>
          <td>Latin America</td>
        </tr>
        <tr>
          <td>2024</td>
          <td><span class="event-type type-panel">Conference</span></td>
          <td>MPSA (Midwest Political Science Association)</td>
          <td>Chicago, IL</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

</div>

<script>
function toggleYear(year) {
  const content = document.getElementById('content-' + year);
  const icon = document.getElementById('icon-' + year);
  
  if (content.classList.contains('collapsed')) {
    content.classList.remove('collapsed');
    content.classList.add('expanded');
    icon.classList.remove('collapsed');
  } else {
    content.classList.add('collapsed');
    content.classList.remove('expanded');
    icon.classList.add('collapsed');
  }
}
</script>
