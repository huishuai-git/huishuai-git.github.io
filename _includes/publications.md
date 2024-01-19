<!-- <h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="journals">
<ol class="bibliography"> -->


<h2 id="publications" style="margin: 20px 0px 10px;">Publications</h2>






<!-- Sub-item "Preprints" under "Publications" -->
<h3 id="arxiv" style="margin: 10px 0px 10px;">PrePrints</h3> <!-- Add this line -->

<div class="arxiv">
<ol class="bibliography">
{% for link in site.data.arxiv.main %}
<li style="margin-bottom: 10px;"> <!-- Adjust the bottom margin to reduce the gap -->
  <div class="pub-row">
    <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
      {% if link.image %} 
      <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
      {% endif %}
      {% if link.conference_short %} 
      <abbr class="badge">{{ link.conference_short }}</abbr>
      {% endif %}
    </div>
    <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
        <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
        <div class="author">{{ link.authors }}</div>
        <div class="periodical"><em>{{ link.journal }}</em></div>
      <div class="links">
        <!-- Link buttons -->
      </div>
    </div>
  </div>
</li>
<!-- Removed the <br> tag here -->
{% endfor %}
</ol>
</div>

<!-- Sub-item "Conferences" under "Publications" -->
<h3 id="conferences" style="margin: 10px 0px 10px;">Conference Proceedings</h3> <!-- Add this line -->

<div class="conferences">
<ol class="bibliography">
{% for link in site.data.conferences.main %}
<li style="margin-bottom: 10px;"> <!-- Adjust the bottom margin to reduce the gap -->
  <div class="pub-row">
    <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
      {% if link.image %} 
      <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
      {% endif %}
      {% if link.conference_short %} 
      <abbr class="badge">{{ link.conference_short }}</abbr>
      {% endif %}
    </div>
    <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
        <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
        <div class="author">{{ link.authors }}</div>
        <div class="periodical"><em>{{ link.conference }}</em></div>
      <div class="links">
        <!-- Link buttons -->
      </div>
    </div>
  </div>
</li>
<!-- Removed the <br> tag here -->
{% endfor %}
</ol>
</div>


<h3 id="journals" style="margin: 10px 0px 10px;">Journals</h3>

<div class="journals">
<ol class="bibliography">
{% for link in site.data.journals.main %}
<li style="margin-bottom: 10px;"> <!-- Adjust the bottom margin to reduce the gap -->
  <div class="pub-row">
    <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
      {% if link.image %} 
      <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
      {% endif %}
      {% if link.journal_short %} 
      <abbr class="badge">{{ link.journal_short }}</abbr>
      {% endif %}
    </div>
    <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
        <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
        <div class="author">{{ link.authors }}</div>
        <div class="periodical"><em>{{ link.journal }}</em></div>
      <div class="links">
        <!-- Link buttons -->
      </div>
    </div>
  </div>
</li>
<!-- Removed the <br> tag here -->
{% endfor %}
</ol>
</div>