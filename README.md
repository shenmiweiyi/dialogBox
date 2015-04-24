# dialogBox

dialogBox is a jQuery plugin of customizable, styleable dialog box.

## Features

* Support custom dialog box style.
* on the high version of brwosers support a series of animation effect
* Support adaptive popup content size
* Support the standard and the modal dialog box
* Support IE7+,Firefox3+,Chrome and Oprea

## Usage

HTML

```
<input  type="button" value="click me" id="btnDialog" />
<div id="dialog"></div> <!-- custom dialog box layer(must defined) -->
```

Link to the **jQuery.js** file:

```
<script src="http://code.jquery.com/jquery-1.11.2.min.js"></script>
```

Link to the **jquery.dialogBox.js** file:

```
<script src="js/jquery.dialogBox.js"></script>
```

Add the **CSS** file:

```
<link rel="stylesheet" type="text/css" href="css/jquery.dialogbox.css">
```

To initialize:

```
$(function(){
	$('#btnDialog').click(function(){
		$('#dialog').dialogBox({
			autoHide: true,
			hasClose: true,
			effect: 'fade',
			hasBtn: true,
			type: 'correct',
			title: 'I am title text',
			content: 'I am a dialog box! Please custom styles base on options!'
		})
	})
})
```

## Notes
The dialogBox plugin will according to match the native select on a page, the automatically generated simulation select, according to the native select the **name** and **id** attribute stored and added to the original list (it does not destroy the native defined properties).
native to the select is **the name and id attribute must be set and must be consistent** (for compatibility linkage select ).

## License

Copyright © 2015 YuChao Liu Licensed under the MIT license.