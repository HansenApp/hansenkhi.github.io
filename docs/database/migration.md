# Migraton
creating the new migrations

```php title=m002_blog.php
<?php

namespace Hansen\database\migrations;

class m002_blog extends \Hansen\system\Database\Migrations
{
    public function up()
    {
        $db = $this->addTable("blog");
        $db->addColumn("title", "string");
        $db->addColumn("body", "string");
    }

    public function down()
    {
        $this->removeTable("blog");
    }
}
```

migrating the all migrations
```shell
php han migrate:fresh
```