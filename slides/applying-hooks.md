### Applying Hooks

WordPress lets you execute custom hooks anywhere you'd like!

```php
do_action( 'some_action_hook' [, $args] );

$value = apply_filters( 'some_filter', $value [, $args] );
```