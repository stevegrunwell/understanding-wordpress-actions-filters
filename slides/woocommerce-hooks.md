### WooCommerce Hooks

```php
# single-product.php

/**
 * woocommerce_before_main_content hook.
 *
 * @hooked woocommerce_output_content_wrapper - 10
 * @hooked woocommerce_breadcrumb - 20
 */
do_action( 'woocommerce_before_main_content' );
```
<!-- .element: class="fragment" -->

Note:

WooCommerce, like many other plugins that integrate with a theme, attaches modules/components to hooks.

One thing they do really well, however, is documenting what's hooked and where.
