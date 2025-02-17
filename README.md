 # Laravel Event Project

This is a Laravel-based project designed for event management. Follow the steps below to set up and run the project on your local system.

## Prerequisites
- PHP (>= 8.0)
- Composer (latest version)
- Node.js & npm (latest LTS recommended)
- MySQL or any other database supported by Laravel
- XAMPP/WAMP (optional for local server setup)

## Installation Steps

### 1. Clone the Repository
```sh
git clone https://github.com/Shankaranarayanansk/IQUD_Event-Laravel.git
cd IQUD_Event-Laravel
```

### 2. Install Dependencies
Run the following command to install PHP dependencies:
```sh
composer install
```

Then, install Node.js dependencies:
```sh
npm install
```

### 3. Set Up Environment Variables
Copy the example environment file and modify it as needed:
```sh
cp .env.example .env
```
Then, update `.env` with your database credentials:
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_db_user
DB_PASSWORD=your_db_password
```

### 4. Generate Application Key
```sh
php artisan key:generate
```

### 5. Run Migrations and Seeders (If Needed)
```sh
php artisan migrate --seed
```

### 6. Start the Development Server
```sh
php artisan serve
```
The application will now be available at `http://127.0.0.1:8000/`.

### 7. Run Vite for Frontend (If using Tailwind or Vue/React)
```sh
npm run dev
```

## Additional Commands

### To Clear Cache
```sh
php artisan cache:clear
php artisan config:clear
php artisan route:clear
php artisan view:clear
```

### To Compile Assets for Production
```sh
npm run build
```

## License
This project is open-source and available under the [MIT License](LICENSE).