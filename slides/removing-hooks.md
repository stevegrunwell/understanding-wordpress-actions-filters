### Removing Hooks

Actions and filters can be removed via `remove_action()` or `remove_filter()`, respectively.

```php
// Adding the hook.
add_action( 'my_action', 'my_callback', 10, 4 );

// Removing the hook.
remove_action( 'my_action', 'my_callback', 10, 4 );
```
<!-- .element: class="fragment" -->

Must be given the same arguments that were passed when the hook was added!<!-- .element: class="fragment" -->

Note:

One of the most frustrating things you'll deal with when using other people's hooks is removing the ones you don't want.

If the arguments don't match exactly the call to remove_hook() will silently fail.
