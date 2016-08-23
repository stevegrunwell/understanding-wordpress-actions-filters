####  Ajax handling

```php
function my_ajax_callback() {
	$value = $_POST['some_key'];

	// Do something with the data.

	echo 'This is my response';
	exit; // or die().
}
```

```
add_action( 'wp_ajax_my_action', 'my_ajax_callback' );

// Logged-out users:
add_action( 'wp_ajax_nopriv_my_action', 'my_ajax_callback' );
```
<!-- .element: class="fragment" -->

Note:

Now that we're POST-ing data, we need something to handle it.

Here we have my_ajax_callback(), which does something with $_POST['some_key'] and gives us the string "This is my response".

Notice that we're exiting the script at the end; this is important to signal to PHP that you've output everything you need to.

Then, we register our callback on the wp_ajax_my_action hook, where "my_action" is the value of the "action" parameter we passed in our data object.

If we need to make this action available to unprivileged users, we'll also add it to the "nopriv" hook as well.
