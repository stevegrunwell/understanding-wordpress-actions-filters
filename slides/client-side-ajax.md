#### Client-side Ajax

```js
var data = {
	action: 'my_action',
	// include other data as appropriate.
};

$.post( ajaxurl, data, function ( response ) {
	// Do something with the response.
} );
```

```js
var ajaxurl = '<?php echo admin_url( 'admin-ajax.php' ); ?>';
```
<!-- .element: class="fragment" -->

Note:

While JavaScript isn't the only way to send requests to admin-ajax.php, it's the most common.

Your most basic implementation will look like this: a data object, where we define an "action" key, then a simple $.get request (though this could be $.post or any other HTTP action). When it finishes, it calls our third argument, which is a callback.

You might notice that `ajaxurl` is seemingly coming out of nowhere. It's automatically defined globally in the admin section, but if you're using this on the frontend you'll need to define it yourself.
