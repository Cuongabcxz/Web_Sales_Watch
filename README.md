# Cài đặt
## Yêu cầu
- PHP 7.4 trở lên
- MySQL 5.7 trở lên
- Laravel 8.0
- Git
- Composer

## Tiến hành
- Chạy các lệnh sau tại đường dẫn lưu source code:
```
git clone https://github.com/Cuongabcxz/Web_Sales_Watch
cd flipper
composer install
php artisan key:generate
cp .env.example .env
```

- Vào phpMyadmin hoặc dùng lệnh MySQL để tạo database `laravel` với character set `utf8mb4` và collate là `utf8mb4_unicode_ci`.  

- Mặc định  file `.env` cấu hình database như bên dưới, nếu có thay đổi gì thì có thể mở file này để chỉnh sửa
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

- Sau đó tại đường dẫn thư mục `laravel` chạy lệnh:
```
php artisan app:reset
```

# Cập nhật
Vào thư mục `laravel`, nếu muốn cập nhật cấu hình thì tham số `env` để là `true`, ngược lại thì `false`.
```
php artisan app:reset --env=true 
```

hoặc

```
php artisan app:reset --env=true
```
