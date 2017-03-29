
# jquery.sharebox

This [jQuery](https://jquery.com/) plugin allow you to easily add a
 *sharebox* (list of social buttons) on your website.

![Screenshot](screenshot.png?raw=true)



## Setup

Simply load jQuery and the provided files from the right place:

```html
<!-- jQuery -->
<script src="path/to/jquery.min.js"></script>

<!-- jquery.sharebox -->
<script src="path/to/jquery.sharebox.min.js"></script>
<link href="path/to/jquery.sharebox.min.css" rel="stylesheet">
```


Note: The optional `jquery.sharebox.icons.css` stylesheet contains all
 icons in the [data URI scheme](https://en.wikipedia.org/wiki/Data_URI_scheme).



## Usage

**jquery.sharebox** will automatically load any `.sharebox` elements:

```html
<!-- .sharebox elements are automatically loaded -->
<div class="sharebox"></div>
```


Off course, you can also initialize **jquery.sharebox** with the element
 you want:

```html
<div id="my-sharebox"></div>
<script>
jQuery(document).ready(function() {
	jQuery("#my-sharebox").sharebox();
});
</script>
```



## Configuration

### Options

**jquery.sharebox** accepts the following options:

| Name     | Description                      | Default value            |
| -------- | -------------------------------- | ------------------------ |
| url      | The URL to share                 | URL of the document      |
| title    | The name of the element to share | Title of the document    |
| services | The services you want to use *   | facebook twitter google+ |

<small>_\* Separated by space_</small>


### The HTML way

With **jquery.sharebox**, you can easily set options using
 [HTML5 custom data attributes](https://www.w3.org/TR/2010/WD-html5-20101019/elements.html#embedding-custom-non-visible-data-with-the-data-attributes).

```html
<!-- .sharebox elements are automatically loaded -->
<div class="sharebox"
     data-url="http://www.example.com/"
     data-title="My awesome title"
     data-services="facebook twitter google+ print"
     ></div>
```


### The javascript way

The **jquery.sharebox** plugin allows you to set options by passing an object
 on initialization:

```html
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
```



## Services

By default, **jquery.sharebox** includes the following services :

* ![Digg](src/icons/digg.png?raw=true) **digg** - Share on [Digg](https://digg.com/)
* ![Facebook](src/icons/facebook.png?raw=true) **facebook** - Share on [Facebook](https://www.facebook.com/)
* ![Google+](src/icons/google-plus.png?raw=true) **google+** - Share on [Google+](https://plus.google.com/)
* ![LinkedIn](src/icons/linkedin.png?raw=true) **linkedin** - Share on [LinkedIn](https://www.linkedin.com/)
* ![Pinterest](src/icons/pinterest.png?raw=true) **pinterest** - Share on [Pinterest](https://pinterest.com/)
* ![Pocket](src/icons/pocket.png?raw=true) **pocket** - Share on [Pocket](https://getpocket.com/)
* ![Reddit](src/icons/reddit.png?raw=true) **reddit** - Share on [Reddit](https://reddit.com/)
* ![StumbleUpon](src/icons/stumbleupon.png?raw=true) **stumbleupon** - Share on [StumbleUpon](https://www.stumbleupon.com/)
* ![Tumblr](src/icons/tumblr.png?raw=true) **tumblr** - Share on [Tumblr](https://www.tumblr.com/)
* ![Twitter](src/icons/twitter.png?raw=true) **twitter** - Share on [Twitter](https://twitter.com/)
* ![Print](src/icons/print.png?raw=true) **print** - Open the _Print Dialog_



## License

Simply [do what the fuck you want](LICENSE "View Licence").
