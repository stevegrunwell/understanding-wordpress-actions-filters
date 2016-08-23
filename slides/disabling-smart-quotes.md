### Disabling "smart" quotes

```php
remove_filter( 'the_content', 'wptexturize' );
```

Note:

One of the first times developers come across filters, it's often to do something like this: disabling the curly (or "smart") quotes in body text.

By default, WordPress registers the `wptexturize()` filter function to run on `the_content()`, but this line will remove it.
