### A noble filter embiggens the smallest post title

```php
// Default behavior.
the_title();
#=> Hello, World!
```

```php
// A perfectly cromulent function name.
function embiggen_text( $text ) {
	return strtoupper( $text );
}
add_filter( 'the_title', 'embiggen_text' );
```
<!-- .element: class="fragment" -->

```php
// Do it again, but with filters!
the_title();
#=> HELLO, WORLD!
```
<!-- .element: class="fragment" -->
