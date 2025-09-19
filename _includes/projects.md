<h2 id="publications" style="margin: 2px 0px 0px;">School/Personal Projects</h2>

<div class="projects" style="padding-top: 15px;">

{% for link in site.data.projects.main %}

<div class="pub-row" style="display: flex; margin-bottom: 20px; align-items: center;">
  <div class="col-sm-3 abbr" style="flex: 0 0 15%; padding-right: 15px; padding-left: 15px;">
    {% if link.image %} 
    <div style="width: 200px; height: 150px; overflow: hidden; margin: 0 auto; border-radius: 10px;">
      <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" 
           style="width: 100%; height: 100%; object-fit: cover; display: block;">
    </div>
    {% endif %}
  </div>
  <div class="col-sm-9" style="flex: 1; padding-right: 15px; padding-left: 20px;">
    <div class="title" style="font-weight: bold; font-size: 18px;">
      <a href="{{ link.pdf }}">{{ link.title }}</a>
    </div>
    <div class="author" style="margin-top: 5px; font-size: 14px;">{{ link.authors }}</div>
    <div class="class" style="font-size: 14px; font-style: italic; margin-top: 5px;">{{ link.class }}</div>
    <div class="links" style="margin-top: 10px;">
    {% if link.pdf %} 
    <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" 
        style="font-size: 12px; border: 1px solid #ffffff; padding: 5px 10px; border-radius: 5px; display: inline-block; text-decoration: none; color: #ffffff;">PDF</a>
    {% endif %}
    {% if link.code %} 
    <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" 
        style="font-size: 12px; border: 1px solid #ffffff; padding: 5px 10px; border-radius: 5px; display: inline-block; text-decoration: none; color: #ffffff;">Code</a>
    {% endif %}
    {% if link.page %} 
    <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" 
        style="font-size: 12px; border: 1px solid #ffffff; padding: 5px 10px; border-radius: 5px; display: inline-block; text-decoration: none; color: #ffffff;">Project Page</a>
    {% endif %}
    </div>
  </div>
</div>

{% endfor %}

</div>
