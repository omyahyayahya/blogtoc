# BlogToc

A javascript plugin to make table of contents for blogspot using Blogger Feed API

### Basic Usage ###

Place this code somewhere in the `<head></head>` section.

```html
<script type="text/javascript" src="//blogtoc2.googlecode.com/svn/trunk/blogtoc.min.js"></script>
```

Then add these codes below in your blog page or post

```html
<div id="YOUR_ID"></div>
 
<script type="text/javascript">
var myDiv = document.getElementById('YOUR_ID');
 
BlogToc( myDiv ).build({
  url: "YOUR_BLOGSPOT_URL.blogspot.com"
});
</script>
```

## Demo ##
http://clusteramaryllis.github.io/blogtoc/

## Compatibility ##
The Javascript Files are being tested in the latest versions of Chrome, Firefox, 
and IE6+ (Partial)

## License ##
http://www.apache.org/licenses/LICENSE-2.0

## External Resources ##
BlogToc using some external service to generate image on the fly

* [boxresizer](http://boxresizer.com/)
* [mobify](http://www.mobify.com/mobifyjs/v2/docs/image-resizer/)
* [sencha](http://www.sencha.com/learn/how-to-use-src-sencha-io/)
* [using google image resizer trick](http://carlo.zottmann.org/2013/04/14/google-image-resizer/)

User interface using [Twitter Bootstrap](http://getbootstrap.com/)

And iconic font from [Bootmetro](http://aozora.github.io/bootmetro)

## Changelog ##

### 1.6.0
* Added dataType option (using JSONP or JSON).
* Added RTL Support (experimental).
* Added number option for parsing the number in index column, pagination, page report.
* Added alphabetMember and symbolicAlphabetRegex for determine the alphabet filter (still buggy).
* Remove theme standalone option (prefered using synchronous request).
* Update bootstrap theme to v3.0.3
* Other theme deprecated except bootstrap.
* Added [json2](https://github.com/douglascrockford/JSON-js) submodule for parsing JSON data.

### 1.5.0
* First Stable Release