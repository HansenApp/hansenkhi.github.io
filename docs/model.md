# Models

## Normal Model

Normal model example

```php
<?php

namespace App\Models;

use Hansen\system\Core\Model;

class Blog extends Model
{
    public function getAllData()
    {
        $this->query("SELECT * FROM blog");
        $this->all();
    }
}

```

## Validation Model

Validation model example

```php
<?php 
 
namespace App\Models; 

use Hansen\system\Core\ValidationModel;

class Blog extends ValidationModel
{
    public $title;
    public $body;

    public function rules(): array
    {
        return [
            'title' => [self::RULE_REQUIRED],
            'body' => [self::RULE_REQUIRED, [self::RULE_MIN, 'min' => 10]],
        ];
    }
}
```