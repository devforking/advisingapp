# config / database

```php
    'connections' => [
        'landlord' => [
            'driver' => 'mysql',
            'port' => env('DB_PORT', '3306'),
            'host' => env('DB_HOST', '127.0.0.1'),
            'database' => env('DB_DATABASE', 'forge'),
            'username' => env('DB_USERNAME', 'forge'),
            'password' => env('DB_PASSWORD', ''),
            'charset' => 'utf8',
            'prefix' => '',
            'prefix_indexes' => true,
            'search_path' => 'public',
            'sslmode' => 'prefer',
        ],

        'tenant' => [
            'driver' => 'mysql',
            'host' => env('TENANT_DB_HOST', '127.0.0.1'),
            'port' => env('TENANT_DB_PORT', '3306'),
            'database' => env('TENANT_DB_DATABASE', ''),
            'username' => env('TENANT_DB_USERNAME'),
            'password' => env('TENANT_DB_PASSWORD'),
            'charset' => 'utf8',
            'prefix' => '',
            'prefix_indexes' => true,
            'search_path' => 'public',
            'sslmode' => 'prefer',
        ],
    ],

```

# env

```bash
DB_DATABASE=advising_landlord
DB_USERNAME=root
DB_PASSWORD=

TENANT_DB_DATABASE=advising_tenant
TENANT_DB_USERNAME=root
TENANT_DB_PASSWORD=
```