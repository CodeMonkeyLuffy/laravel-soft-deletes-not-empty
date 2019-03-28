# Laravel SoftDeletes With Unix Timestamp

## Installing

```sh
$ composer require CodeMonkeyLuffy/laravel-soft-deletes
```


## Usage

```php
<?php

namespace App;

use Illuminate\Database\Eloquent\Model;
use CodeMonkeyLuffy\LaravelSoftDeletes\Eloquent\SoftDeletes;

class Car extends Model
{

    use SoftDeletesNotEmpty;

    protected $dateFormat = 'U';

    protected $dates = ['deleted_at'];
}
```

## License

MIT