### Argument Count

The number of arguments that should be passed to the callback. Default is 1.

```php
function my_callback( $foo, $bar, $baz ) {
	// Do something.
}

add_action( 'my_hook', 'my_callback', 10, 3 );
```

Note:

Of course, we can't pass more arguments we're passing when we call do_action() or apply_filters().