---
layout: default
---





{% layout layout: "container" cid: "div_id" cname: "container_extra_class" "%}


{% layout layout: "row" cid: "row_id" cname: "row_extra_class" "%}

{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 1
<a href="#">I am a link</a>
{% endlayout %}
{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 2
{% endlayout %}
{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 3
{% endlayout %}

{% endlayout %}

{% endlayout %}