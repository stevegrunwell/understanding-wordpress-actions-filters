#### Removing method callbacks

In order to remove method callbacks, you need the original instance.

```php
// Inside some object method:
add_action( 'my_action', [ $this, 'my_callback' ], 10, 4 );
```
<!-- .element: class="fragment" -->

```php
// Can't remove the action on a different instance.
$instance = new MyObject;
remove_action( 'my_action', [ $instance, 'my_callback' ], 10, 4 );
```
<!-- .element: class="fragment" -->

<!-- .element: class="fragment" -->Common (less-than-awesome) pattern is to store the `$instance` as a global variable.

Note:

When you register a callback on a method of $this,

Object-oriented vs. namespaced, procedural code is outside the scope of this talk, but this is another reason procedural code is preferable.

