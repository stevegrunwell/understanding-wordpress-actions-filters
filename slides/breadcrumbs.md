#### We can remove breadcrumbs, &hellip;

```php
remove_action(
	'woocommerce_before_main_content',
	'woocommerce_breadcrumb',
	20
);
```
