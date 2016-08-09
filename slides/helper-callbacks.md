#### Built-in Callbacks

```php
// Booleans.
__return_true()         === true;
__return_false()        === false;

// Integers, null, strings, and arrays.
__return_zero()         === 0;
__return_null()         === null;
__return_empty_string() === '';
__return_empty_array()  === array();
```

```php
add_filter( 'some_filter', '__return_false' );
```
<!-- .element: class="fragment" -->
