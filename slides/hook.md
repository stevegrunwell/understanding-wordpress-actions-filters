### Hook

The `$hook` identifies the action or filter.

```php
add_filter( 'the_content', ... );
add_action( 'wp_footer', ... );
add_action( 'save_post-my-post-type', ... );
```
<!-- .element: class="fragment" -->

Note:

Hooks can be created dynamically, making it very easy for plugins to call them on the off-chance a