---
layout: default
---





{% layout layout: "bootstrap/container" cid: "div_id" cname: "container_extra_class" "%}


{% layout layout: "bootstrap/row" cid: "row_id" cname: "row_extra_class" "%}

{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 1
<a href="#">I am a link</a>
{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 2
{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 3
{% endlayout %}

{% endlayout %}

{% endlayout %}


{% include bootstrap/labels.html  %}

{% layout layout: "bootstrap/section" cid: "div_id" cname: "container_extra_class" "%}
# Inside of the Bootstrap folder
{% endlayout %}
