<!-- <h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="journals">
<ol class="bibliography"> -->


<h2 id="publications" style="margin: 20px 0px 10px;">Publications</h2>
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





<!-- <h2 id="conferences" style="margin: 2px 0px -15px;">Conferences</h2>
<div class="conferences">
<ol class="bibliography"> -->

<!-- Sub-item "Journals" under "Publications" -->
<h3 id="conferences" style="margin: 10px 0px 10px;">Conference Proceedings</h3> <!-- Add this line -->

<div class="conferences">
    <ol class="bibliography">
        <!-- The rest of your code for listing the publications -->
    </ol>
</div>

{% for link in site.data.conferences.main %}

<li>
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
      <div class="periodical"><em>{{ link.conference }}</em>
      <!-- <div class="periodical"><em>{{ link.journal }}</em> -->
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>