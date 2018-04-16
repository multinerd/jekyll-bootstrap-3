# Jekyll Bootstrap 3

This is a simple breakdown of Bootstrap 3 components broken down for use within Jekyll.


## Breakdown


### section
- variables: cname, cid (section class, section id)
```html
<section class="container {{cname}}" id="{{ cid }}">
  {{ content }}
</section>
```

### container
- variables: cname, cid (class, id )
```html
<div class="container {{cname}}" id="{{ cid }}">
  {{ content }}
</div>
```

### row
- variables: cname, cid (class, id )
```html
<div class="row {{cname}}" id="{{ cid }}">
  {{ content }}
</div>
```

### column
- variables: cname, cid (class, id )
```html
<div class="{{cname}}" id="{{ cid }}">
  {{ content }}
</div>
```

### Example
The following is example usage. You can create:
```html
<div class="container" id="container_id">
	<div class="row" id="row_id">
  		<div class="col-sm-4" id="column_id">
  			<h1>Header Column 1</h1>
		</div>
		<div class="col-sm-4" id="column_id">
  			<h1>Header Column 2</h1>
		</div>
		<div class="col-sm-4" id="column_id">
  			<h1>Header Column 3</h1>
		</div>
	</div>
</div>
```


and now with templating as:
````
{% layout layout: "container" cid: "div_id" cname: "container_extra_class" "%}


{% layout layout: "row" cid: "row_id" cname: "row_extra_class" "%}

{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 1
{% endlayout %}
{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 2
{% endlayout %}
{% layout layout: "column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 3
{% endlayout %}

{% endlayout %}

{% endlayout %}
````