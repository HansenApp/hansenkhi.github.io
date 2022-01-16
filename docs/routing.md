# Routing

ok, If you have initialized your **application**, now you can continue the route. to the configure the route you can open file in `ROOT_DIR/routes/main.php`. it will show

```php title=main.php
<?php

use Hansen\system\Core\Route;
use Hansen\system\Core\View;

$router = new Route();

$router->get("/", function () {
    return View::render('index');
});

$router->run();
```

adding the new routes

```php
// GET Method
$route->get("/", function() {
    return 'Hello, World!';
});

// POST Method

$route->post("/", function() {
    return 'Hello, World!';
});
```