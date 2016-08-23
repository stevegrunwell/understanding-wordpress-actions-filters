### Adding tracking scripts to the site footer

```php
function add_tracking_scripts() {
?>

	<script>
		// Some third-party tracking script.
	</script>

<?php
}
add_action( 'wp_footer', 'add_tracking_scripts' );
```

Note:

This is a really popular use of the wp_footer action: adding third-party tracking scripts like Simply Measured, Omniture, etc.

Can also be accomplished via text widgets if your theme supports them, but this gives a cleaner implementation that non-developers can't accidentally delete.
