
# jquery.sharebox

This [jQuery](https://jquery.com/) plugin allow you to easily add a
 *sharebox* (list of social buttons) on your website.

[![Screenshot](screenshot.png?raw=true)](https://rawgit.com/Seebz/jquery.sharebox/master/demo.html "View live demo")



## Getting started

### Setup

Simply load jQuery and the provided files from the right place:

	<!-- jQuery -->
	<script src="path/to/jquery.min.js"></script>

	<!-- jquery.sharebox -->
	<script src="path/to/jquery.sharebox.min.js"></script>
	<link href="path/to/jquery.sharebox.min.css" rel="stylesheet">


Note: The optional `jquery.sharebox.icons.css` stylesheet contains all
 icons in the [data URI scheme](https://en.wikipedia.org/wiki/Data_URI_scheme).


### Usage

**jquery.sharebox** will automatically load any `.sharebox` elements:

	<!-- .sharebox elements are automatically loaded -->
	<div class="sharebox"></div>


Off course, you can also initialize **jquery.sharebox** with the element
 you want:

	<div id="my-sharebox"></div>
	<script>
	jQuery(document).ready(function() {
		jQuery("#my-sharebox").sharebox();
	});
	</script>


### Configuration

#### Options

**jquery.sharebox** accepts the following options:

| Name     | Description                      | Default value            |
| -------- | -------------------------------- | ------------------------ |
| url      | The URL to share                 | Document's URL           |
| title    | The name of the element to share | Document's title         |
| services | The services you want to use *   | facebook twitter google+ |
| -------- | -------------------------------- | ------------------------ |
* Separated by space


#### The HTML way

With **jquery.sharebox**, you can easily set options using
 [HTML5 custom data attributes](https://www.w3.org/TR/2010/WD-html5-20101019/elements.html#embedding-custom-non-visible-data-with-the-data-attributes).

	<!-- .sharebox elements are automatically loaded -->
	<div class="sharebox"
	     data-url="http://www.example.com/"
	     data-title="My awesome title"
	     data-services="facebook twitter google+ print"
	     ></div>


#### The javascript way

The **jquery.sharebox** plugin allows you to set options by passing an object
 on initialization:

	<div id="my-sharebox"></div>
	<script>
	jQuery(document).ready(function() {
		jQuery("#my-sharebox").sharebox({
			url      : "http://www.example.com/",
			title    : "My awesome title",
			services : "facebook twitter google+ print"
		});
	});
	</script>



## License

Simply [do what the fuck you want](LICENSE "View Licence").
