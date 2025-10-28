# E-Commerce Platform

<p align="center">
  <img src="https://laravel.com/img/logomark.min.svg" width="80" alt="Laravel Logo">
</p>

<p align="center">
  <a href="https://laravel.com" target="_blank"><img src="https://img.shields.io/badge/Laravel-11.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel Version"></a>
  <a href="https://php.net" target="_blank"><img src="https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Version"></a>
  <a href="https://laravel.com" target="_blank"><img src="https://img.shields.io/badge/Made%20with-Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Made with Laravel">
</p>

A comprehensive e-commerce platform built with Laravel, featuring product management, user authentication, shopping cart, payment processing, and order management.

## Features

- **Product Management**: Catalog with categories, filters, and search capabilities
- **Shopping Cart**: Persistent cart with multiple items and quantities
- **User Authentication**: Registration, login, password reset, and account management
- **Order Processing**: Complete order lifecycle with status tracking
- **Payment Integration**: Secure payment processing (Stripe/Mollie)
- **Admin Panel**: Dashboard for managing products, orders, and users
- **Responsive Design**: Mobile-friendly interface

## Technologies Used

- **Backend**: Laravel 11.x
- **Frontend**: Blade templates, Tailwind CSS
- **Database**: MySQL
- **Authentication**: Laravel Sanctum / Laravel Fortify
- **Queue System**: Laravel Queues for background processing
- **File Storage**: Laravel Storage for product images
- **Testing**: PHPUnit and Laravel Dusk

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/eCommerce_laravel.git
   cd eCommerce_laravel
   ```

2. Install PHP dependencies:
   ```bash
   composer install
   ```

3. Install Node.js dependencies:
   ```bash
   npm install
   ```

4. Copy the environment file and set appropriate configuration:
   ```bash
   cp .env.example .env
   ```

5. Generate application key:
   ```bash
   php artisan key:generate
   ```

6. Configure your database settings in the `.env` file

7. Run database migrations:
   ```bash
   php artisan migrate --seed
   ```

8. Build assets:
   ```bash
   npm run build
   # or for development with hot reload:
   npm run dev
   ```

9. Start the development server:
   ```bash
   php artisan serve
   ```

## Environment Variables

Create a `.env` file with the following required variables:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_username
DB_PASSWORD=your_database_password

MAIL_MAILER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null
MAIL_FROM_ADDRESS="hello@example.com"
MAIL_FROM_NAME="${APP_NAME}"

STRIPE_KEY=your_stripe_public_key
STRIPE_SECRET=your_stripe_secret_key
```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Testing

Run the test suite:

```bash
php artisan test
```



## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).


