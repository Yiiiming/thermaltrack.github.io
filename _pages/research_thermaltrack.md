---
layout: single
author_profile: true
header:
  image: image/rgb_thermal_prediction_159_wider.png
  image_width: 800   # Must match CSS
  image_height: 200

---
{% include base_path %}

<h3>Motivation</h3>

<h5><span style="font-weight:normal">Autonomous systems struggle in snow-covered environments where visual cues disappear and terrain properties become homogeneous. Traditional perception systems fail to leverage the most reliable navigation cues available in these conditions: the physical imprint of previously traversed paths. This research addresses the critical need for robust wheel track detection to enable safe winter autonomy.</h5>

<h3>Solution</h3>

<h5><span style="font-weight:normal">Following existing wheel tracks provides verified path stability, predictable vehicle dynamics through compacted snow, and higher traction from pre-deformed terrain. These physical advantages persist even in white-out conditions, offering a failsafe navigation solution when other features vanish.</h5>

<h3>Methods</h3>

<h5><span style="font-weight:normal">We present a wheel track detection system that leverages RGB-Thermal (RGB-T) imaging, where thermal channels reveal critical temperature differentials between tracks and snow, enabling wheel track detection in complete white-out conditions.</h5>
<img src="{{ '/image/model_comparison.png' | relative_url }}" alt="Model Comparison">

<div class="grid__wrapper">
  {% for post in paginator.posts paginate:8 %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

{% include paginator.html %}

<!-- 
<h2 class="archive__subtitle">AutoRally software on GitHub</h3>

<iframe src="https://ghbtns.com/github-btn.html?user=autorally&repo=autorally&type=watch&count=true&size=large&v=2" frameborder="0" scrolling="0" width="160px" height="30px" align="middle"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=autorally&repo=autorally&type=star&count=true&size=large" frameborder="0" scrolling="0" width="160px" height="30px" align="middle"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=autorally&repo=autorally&type=fork&count=true&size=large" frameborder="0" scrolling="0" width="158px" height="30px" align="middle"></iframe>
-->
