### Filtering post titles

```php
/**
 * Prepend posts in the "Breaking News" category with "Breaking:".
 *
 * @param string $title The post title.
 * @param int    $id    The post ID.
 * @return The filtered $title.
 */
function prepend_breaking_news( $title, $id ) {
	if ( has_category( 'Breaking News', $id ) ) {
		$title = 'Breaking: ' . $title;
	}

	return $title;
}
add_action( 'the_title', 'prepend_breaking_news', 10, 2 );
```