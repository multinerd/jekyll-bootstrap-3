# Jekyll Bootstrap 3
------
Seperate code from content using this.  Render bootstrap-able components via a smart template plugin.

## Requirements
------
- You need to have **bootstrap** (doesn't matter how you install it as long as you have the css file.)
- You need to include the **layout_template.rb** into your **_plugins** directory.
- Add the **bootstrap** folder into your **_includes** folder. 





## Breakdown
------
### section
Variables: cname, cid (section class, section id)
```html
<section class="container {{cname}}" id="{{ cid }}">
  {{ content }}
</section>
```

### container
Variables: cname, cid (class, id )
```html
<div class="container {{cname}}" id="{{ cid }}">
  {{ content }}
</div>
```

### row
Variables: cname, cid (class, id )
```html
<div class="row {{cname}}" id="{{ cid }}">
  {{ content }}
</div>
```

### column
Variables: cname, cid (class, id )
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


using jekyll boostrap template it would look like this:
````
{% layout layout: "bootstrap/container" cid: "div_id" cname: "container_extra_class" "%}


{% layout layout: "bootstrap/row" cid: "row_id" cname: "row_extra_class" "%}

{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 1
{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 2
{% endlayout %}
{% layout layout: "bootstrap/column" cname: "col-sm-4" cid: "column_id"  "%}
# Header column 3
{% endlayout %}

{% endlayout %}

{% endlayout %}
````


### buttons
Theres a few types to select from: anchor, button, input, submit
````
{% include bootstrap/button.html 
	button_type="anchor" 
	link="http://richardchiriboga.com" 
	cid="btn_id" 
	cname="btn btn-default" 
	txt="click here to..." 
%}
````

### youtube
Easily add a youtube video responsively embedded to any page
````
{% include bootstrap/youtube.html video_id ="cRZOgd7mcY8" %}
````


### Unordered / Ordered Lists
Each one works the exact way. ul / ol respectively.
````
{% include bootstrap/undordered_list.html cname ="class" cid="your_id" %}
````
````
{% include bootstrap/ordered.html cname ="class" cid="your_id" %}
````


### Labels
Each one works the exact way. ul / ol respectively.
```html
{% include bootstrap/label.html cname ="class" cid="your_id" %}
{% include bootstrap/ordered.html cname ="class" cid="your_id" %}
```
