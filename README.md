# registry

```php
<?php
use GuzzleHttp\Client;

$registry = json_decode((new Client)->get('https://larawal.github.io/registry/registry.json'), true);

if (isset($registry['ecommerce'])) {
  // 
}
```

