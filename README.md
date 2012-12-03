Prototype.AJAXMGraph
====================

Mirrored from http://dragan.yourtree.org/code/ajax-mgraph/


__ABOUT__

As you can see this is simple bar-graph that shows data by month. Soon I'll release other graph to complete this package (daily, and hourly graph).
Also I will release one universal graph that plots any given data. Stay tuned for more...

__HOW TO SETUP__

Download Archive

Extract files to some remote or local directory

Include `agGraph.css` file in your page

```html
<link rel="stylesheet" type="text/css" media="screen" href="agGraph.css" />
```

Download and include [prototype.js](http://prototypejs.org/download) file in your page
Include `graphM.prototype.js` file in your page


```html
<script type='text/javascript' src='prototype.js'></script>
<script type='text/javascript' src='graphM.prototype.js'></script>
```

Define destination DIV, and write note title and text

```javascript
	var graph1={
		divID:'resultDiv1',
		ShowNote:'yes',
		NoteTitle:'Note',
		NoteText:'Little note about this graph goes here...'
	}
	
	var graph2={
		divID:'resultDiv2',
		ShowNote:'yes',
		NoteTitle:'Note',
		NoteText:'Now with multiple graphs :)'
	}
```

Add `onclick="draw();"` to some element

```html
<input type="button" value="Generate Graph" id="startButton" onclick="draw();" />
```

Edit `number_generator.php`, and enter your values there or provide data from database, xml, remote file....