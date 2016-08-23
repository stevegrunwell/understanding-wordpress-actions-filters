#### &hellip; or do something entirely new!

```php
remove_action(
	'woocommerce_before_main_content',
	'woocommerce_breadcrumb',
	20
);

// Call my_awesome_breadcrumbs() instead.
add_action(
	'woocommerce_before_main_content',
	'my_awesome_breadcrumbs',
	20
);
```
