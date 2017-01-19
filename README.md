# Summernote Accordion

Plugin to add a bootstrap 3 accordion with summernote <http://summernote.org>

### Installation and dependencies

Summernote Accordion uses opensource libraries: [Summernote](http://summernote.org/), [jQuery](http://jquery.com/), [Bootstrap](http://getbootstrap.com).

#### 1. include JS/CSS

Include the following code in the `<head>` tag of your HTML:

```html
<!-- include libraries(jQuery, bootstrap) -->
<script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script> 
<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.5/css/bootstrap.min.css" />
<script type="text/javascript" src="//cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.5/js/bootstrap.min.js"></script>

<!-- include summernote css/js-->
<link href="summernote.css" rel="stylesheet">
<script src="summernote.js"></script>
<script src="summernote-accordion.js"></script>
```

#### 2. target a element

Then place a `div` tag somewhere in the `body` tag. This element will be replaced with the summernote editor.

```html
<div id="summernote">Hello Summernote</div>
```

#### 3. summernote

Finally, run this script after the DOM is ready:

```javascript
$(document).ready(function() {
  $('#summernote').summernote({
      toolbar: [
        ...
        ['misc', ['accordion']]
      ],
    });
});
```

### License
summernote-accordion may be freely distributed under the MIT license developped by Decasoft.
