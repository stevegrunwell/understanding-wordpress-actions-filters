###  Priority

The order in which callbacks should be executed. Default is 10.

```php
// Will execute first.
add_action( 'my_action', 'my_first_callback', 10 );

// Will execute second.
add_action( 'my_action', 'my_second_callback', 11 );

// Will execute last.
add_action( 'my_action', 'my_last_callback', 9999 );
```
<!-- .element: class="fragment" -->

Note:

It doesn't matter what order we call add_action(), they're added to the queue in order of priority.

If multiple callbacks are added to the same hook with the same priority, they'll be run in the order they were added.
