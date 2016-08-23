### Callback

The `$callback` is the function that should be called when the hook is executed.

```php
// Call a regular function.
add_action( 'my_action', 'my_callback' );

// Class methods.
add_action( 'my_action', array( $object, 'my_callback' ) );

// Function in current namespace.
add_action( 'my_action', __NAMESPACE__ . '\my_callback' );
```
<!-- .element: class="fragment" -->