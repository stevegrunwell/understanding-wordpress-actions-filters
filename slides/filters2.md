### A noble filter embiggens the smallest post title

```php
// Default behavior.
the_title();
#=> Hello, World!
```

```php
function embiggen_text( $text ) {
	return strtoupper( $text );
}
add_filter( 'the_title', 'embiggen_text' );
```

```php
// Do it again, but with filters!
the_title();
#=> HELLO, WORLD!
```