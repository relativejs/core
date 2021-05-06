# RelativeJS
A new approach that looks classic.
This library is focused on bringing a new way of looking at front-end web development.
No build process required.


## Basics
```html
<script src='../assets/relative/relative.js'></script>

<!-- a component definition, via function call -->
<script>
DEFINE_BEHAVIOR(
	// any css selector is valid
	'selector',

	// a function to be called as soon 
	function() { 
		// use vanilla js to do what you gotta do
		this.innerHTML = `Hello ${ this.getAttribute('name') }`
	},

	// the styles to be applied
	`
		background: #a00;
		color: #fff;
	`
)
</script>


<!-- the html itself -->
<selector name='Harry'></selector>
```


## Motivation
There was a time that web development was way simpler: Write a file on any editor you have, save it, refresh the browser. As the web became more powerful it also became increasingly complex and bloated with many frameworks trying to do the same thing in very simliar ways.



## How it works
You define a CSS selector to be listened to. Every time an element is created and it matches that selector, your function will be called and the style will be attatched. How is it helpful?
- any selector valid CSS selector can be used
	- no more limit to only tag names with dashes like HTML5's Custom Components
	- descriptive html
	- tags, subtags, attributes, classes, ids, or a combination of it all. go nuts
- no need for a separate CSS file to define the styles of your components





