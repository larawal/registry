# Larawal registry

The offical list of managed brick by Larawal community

```php
<?php
use GuzzleHttp\Client;

$registry = json_decode((new Client)->get('https://larawal.github.io/registry/registry.json'), true);

$brick = 'ecommerce';
$brick = $registry['shortcuts'][$brick] ?? $brick;

if (isset($registry['bricks'][$brick])) {
  // Yet another e-commerce for my client
}
```
