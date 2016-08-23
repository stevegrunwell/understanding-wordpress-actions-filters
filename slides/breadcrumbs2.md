#### &hellip;Move breadcrumbs, &hellip;

```php
remove_action(
	'woocommerce_before_main_content',
	'woocommerce_breadcrumb',
	20
);

// Remember: woocommerce_output_content_wrapper was priority 10.
add_action(
	'woocommerce_before_main_content',
	'woocommerce_breadcrumb',
	9
);
```
