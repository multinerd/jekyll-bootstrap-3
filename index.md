---
layout: default
---


<!--- container -->
{% layout layout: "bootstrap/container" cid: "div_id" cname: "container_extra_class" "%}


<!--- row -->
{% layout layout: "bootstrap/row" cid: "row_id" cname: "row_extra_class" "%}
<!--- column -->
{% layout layout: "bootstrap/column" cname: "col-sm-12" cid: "column_id"  "%}
## jumbotron
{% layout layout: "bootstrap/jumbotron" cname: "" cid: "column_id"  "%}
# Jumbotron
## Some second header
{% endlayout %} <!--- End of jumbotron -->
{% endlayout %} <!--- End of column -->
{% endlayout %} <!--- End of row -->



<!--- row -->
{% layout layout: "bootstrap/row" cid: "row_id" cname: "row_extra_class" "%}
<!--- column -->
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
<!--- navigation -->
{% layout layout: "bootstrap/unordered_list" cname: "list-group" cid: ""  "%}
<li class="list-group-item"><a href="#">Cras justo odio</a></li>
<li class="list-group-item"><a href="#">Cras justo odio</a></li>
<li class="list-group-item"><a href="#">Cras justo odio</a></li>
<li class="list-group-item"><a href="#">Cras justo odio</a></li>
<li class="list-group-item"><a href="#">Cras justo odio</a></li>
{% endlayout %}<!--- End of nav -->

{% endlayout %} <!--- End of column -->

<!--- column -->
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}

{% endlayout %} <!--- End of column -->


{% endlayout %} <!--- End of row -->
{% endlayout %} <!--- End of container -->




{% layout layout: "bootstrap/container" cid: "div_id" cname: "container_extra_class" "%}


{% layout layout: "bootstrap/row" cid: "row_id" cname: "row_extra_class" "%}

{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}


## Image
{% include bootstrap/image.html src="http://richardchiriboga.com/img/corrientelatina.jpg" cname="img-responsive" %}


{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 2
{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 3
{% endlayout %}

{% endlayout %}

{% endlayout %}





### Unordered List
{% layout layout: "bootstrap/unordered_list" cname: "" cid: ""  "%}
<li>I am an unordered list</li>
<li>I can be a jekyll loop</li>
<li>anything really.</li>
{% endlayout %}


### Ordered List
{% layout layout: "bootstrap/ordered_list" cname: "" cid: ""  "%}
<li>I am an unordered list</li>
<li>I can be a jekyll loop</li>
<li>anything really.</li>
{% endlayout %}


## Labels
{% include bootstrap/labels.html cname="label label-default" txt="Default"  %}

{% include bootstrap/labels.html cname="label label-primary" txt="Primary"  %}

{% include bootstrap/labels.html cname="label label-success" txt="Success"  %}

{% include bootstrap/labels.html cname="label label-info" txt="Info"  %}

{% include bootstrap/labels.html cname="label label-warning" txt="Warning"  %}

{% include bootstrap/labels.html cname="label label-danger" txt="Danger"  %}





{% layout layout: "bootstrap/section" cid: "div_id" cname: "container_extra_class" "%}
# Inside of the Bootstrap folder
{% endlayout %}
