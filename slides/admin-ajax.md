### AJAX in WordPress

WordPress routes all Ajax commands through a single entry point: `wp-admin/admin-ajax.php`

```php
// For logged-in users.
do_action( 'wp_ajax_{action}' );

// For anonymous users.
do_action( 'wp_ajax_nopriv_{action}' );
```
<!-- .element: class="fragment" -->

Note:

All Ajax requests in WordPress end up going through a single file, wp-admin/admin-ajax.php.

This file spins up WordPress, then fires the appropriate actions.