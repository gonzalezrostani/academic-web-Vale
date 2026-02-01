+++
# A Demo section created with the Blank widget.
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 65  # Order that this section will appear.

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
          <td>March 20-22</td>
          <td><span class="event-type type-panel">Panel</span></td>
          <td>Midwest Political Science Association <span class="scheduled-tag">(scheduled)</span></td>
          <td>Chicago, IL, USA</td>
        </tr>
        <tr>
          <td>February 14</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="#">Love of Variety? Experimental Study of Foreign Brands</a> - <i>Political Science Research and Methods</i></td>
          <td>Online First</td>
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
          <td>July 17</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://journals.sagepub.com/doi/10.1177/13684302251346402">Group Process & Intergroup Relations</a></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>July 8</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://www.nature.com/articles/s41597-025-05353-6">Nature: Scientific Data</a></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>June 26</td>
          <td><span class="event-type type-panel">Panel</span></td>
          <td>Public Management Research Conference (PMRC)</td>
          <td>Seoul, South Korea</td>
        </tr>
        <tr>
          <td>April 1</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://onlinelibrary.wiley.com/doi/full/10.1002/pam.70007">Journal of Policy Analysis and Management</a></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>March 17</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://www.cambridge.org/core/journals/journal-of-experimental-political-science/article/solidarity-between-people-of-color-two-blockage-experiments-suggest-it-is-causal-and-resistant-to-a-divisive-threat/3CEAFE3E375FD48D7B5235917CB91D51">Journal of Experimental Political Science</a></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>January 20</td>
          <td><span class="event-type type-talk">Talk</span></td>
          <td>Joined USC as Assistant Professor</td>
          <td>Los Angeles, CA, USA</td>
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
          <td>December</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12481">Social Media vs Surveys</a> - <i>Legislative Studies Quarterly</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>October</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="http://doi.org/10.1111/ecpo.12307">Engaged Robots, Disengaged Workers</a> - <i>Economics & Politics</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>September</td>
          <td><span class="event-type type-publication">Publication</span></td>
          <td><a href="https://onlinelibrary.wiley.com/doi/10.1111/lsq.12476">Legislators' Moral and Economic Policies</a> - <i>Legislative Studies Quarterly</i></td>
          <td>Online First</td>
        </tr>
        <tr>
          <td>June</td>
          <td><span class="event-type type-award">Award</span></td>
          <td>Completed PhD in Political Science</td>
          <td>University of Pittsburgh</td>
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
