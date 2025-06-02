# 🔐 Secure Laravel API with JWT Token & Live Search (No Login)

This is a secure Laravel 12 API-based project where access is granted using a **fixed secret key**, **service name**, and a **JWT token** — without requiring user registration or login. The project includes a frontend interface with a live search functionality to explore services.

## 🚀 Features

✅ Custom JWT token-based API authentication  
✅ Secret key and service name validation  
✅ Token expiry handling with auto-refresh  
✅ Live Search (Frontend) using Bootstrap/Tailwind  
✅ CRUD operations for services (Add/Edit/Delete)  
✅ Modern UI with search suggestions and service cards  
✅ API access restricted only to valid service + token + key  

---

## 🔎 Live Search UI

- A black-themed search bar provides real-time suggestions from the backend API.
- Service cards are shown below with name, icon, and description.
- Users can click on suggestions to view service details.
- Includes "clear search history" button below suggestions.

---

## 🔐 Authentication Flow

1. A fixed **secret key** is stored in `.env`.
2. A token is generated using the key and service name.
3. Token is validated before each API call.
4. Expired tokens are auto-refreshed if the service + key is valid.

---

## 📂 Tech Stack

- Laravel 12 (API)
- Bootstrap 5 / Tailwind (Frontend)
- JavaScript (AJAX for search)
- JWT Token (Custom system)
- MySQL (Database)

---

## 📸 Screenshots

![image](https://github.com/user-attachments/assets/3bfcfcf8-117e-4c85-aeff-8a9ed4b54377)
![image](https://github.com/user-attachments/assets/b5a29d79-bca2-457c-9575-bd7ff1236316)
![image](https://github.com/user-attachments/assets/86873249-f594-4bc0-983a-50b137942855)



---

## ⚙️ Setup Instructions

```bash
git clone https://github.com/mosta82/bKash-Merchant-App-Implementation-of-Search-Button.git
cd secure-laravel-api
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve
