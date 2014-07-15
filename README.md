WordPress Snippets
==

## Gravity Forms

`Change Default Spinner`

```php
/**
 * Changes the default Gravity Forms AJAX spinner.
 *
 * @param string $src The default spinner URL
 * @return string $src The new spinner URL
 */
add_filter('gform_ajax_spinner_url', 'tp_custom_gforms_spinner');
function tp_custom_gforms_spinner($src) {
	return get_template_directory_uri() . '/images/ajax-loader.gif';
}
```
