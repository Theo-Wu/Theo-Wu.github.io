<h2 id="experiences" style="margin: 2px 0px 10px;">Experience</h2>

<div class="experiences">
<ul class="bibliography" style="list-style-type: none; padding-left: 0; margin: 0;">

{% for exp in site.data.experiences.main %}
<li style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <!-- 左侧 Logo -->
  <div style="flex: 0 0 120px; text-align: center; padding-right: 25px; margin-top: 10px;">
    {% if exp.image %}
    <img src="{{ exp.image }}" alt="{{ exp.company }}" style="max-width:100px; height:auto; display:block; margin: 0 auto 15px;">
    {% endif %}
  </div>

  <!-- 右侧文本 -->
  <div style="flex: 1;">
    <div style="font-weight: 500; font-size: 16px;">{{ exp.company }}</div>
    <div style="color: #000000ff; font-weight: 600; font-size: 15px;">{{ exp.position }}</div>
    <div style="color: #555; font-size: 14px; margin-top: 3px;">{{ exp.date }}</div>
    {% if exp.description %}
    <p style="margin-top: 6px; font-size: 14px; color: #444;">{{ exp.description }}</p>
    {% endif %}
  </div>
</li>
{% endfor %}

</ul>
</div>
