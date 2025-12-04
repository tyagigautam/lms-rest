## Setup Guide

Perform the following steps to setup locally.

- **Setup env file** : cp .env.example .env
- **Build and Start containers** : docker-compose up -d --build
- **Generate Key** : docker-compose exec lms_app php artisan key:generate
- **Database setup** : 
  - Access pgAdmin:
    - URL: http://localhost:5050
    - Login Credentials:
      - Email: admin@admin.com 
      - Password: admin
- **Run the migrations** : docker-compose exec lms_app php artisan migrate
- **Access Your Application** : Open your browser and visit: http://localhost:8000
