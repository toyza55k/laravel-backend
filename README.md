# laravel-backend
Laravel backend with AdminLTE 3 

## Installation
1. ```git clone https://github.com/toyza55k/laravel-backend.git```
1. ```composer install```
1. ```
	uncomment in config/app.php
	'providers' => [
		.
		.
		- Yajra\DataTables\DataTablesServiceProvider::class,
    	- Spatie\Permission\PermissionServiceProvider::class,
    'alias' => [
    	.
    	.
    	- 'DataTables' => Yajra\DataTables\Facades\DataTables::class,
    ]
    ```
1. ```
	php artisan migrate:fresh --seed
	or 
	php artisan migrate
	php artisan db:seed
	```
1. ```npm install```
1. ```php artisan storage:link```

### Task Schedules
for removing activity log and force delete rows in trash.
1. ```* * * * * cd /path-to-your-project && php artisan schedule:run >> /dev/null 2>&1```

### Production with shared host
in .env  file
```
FILESYSTEM_DRIVER=public_share_hosted
MEDIA_DISK=public_share_hosted
```

### use composer package
- spatie/laravel-activitylog
- maatwebsite/excel
- spatie/laravel-medialibrary
- spatie/laravel-permission
- spatie/laravel-view-models
- tightenco/quicksand
- yajra/laravel-datatables-oracle

### use npm package
- admin-lte
- inputmask
- jquery-validation
- ladda
- toastr

### adminLTE 
- document https://adminlte.io/docs/3.0/index.html
- demo https://adminlte.io/themes/v3/index.html
