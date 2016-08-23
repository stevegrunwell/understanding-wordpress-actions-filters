### Enabling sites to bypass functionality

```php
if ( apply_filters( 'do_something_optional', '__return_true' ) ) {
	// Do something that maybe not every user would want.
}
```

```php
// Opt-out of the optional feature.
add_filter( 'do_something_optional', '__return_false' );
```
<!-- .element: class="fragment" -->

Note:

This is a very common pattern in well-built plugins: we run `apply_filters()` for a hook with a default value of true (or false, if we'd rather make it opt-in instead of opt-out).

Users can then add a single line to their theme/plugin to bypass the functionality based on this hook.
