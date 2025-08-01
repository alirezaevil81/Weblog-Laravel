# پروژه وبلاگ با لاراول (Weblog-Laravel)

[![Run Laravel Tests](https://github.com/alirezaevil81/Weblog-Laravel/actions/workflows/laravel.yml/badge.svg)](https://github.com/alirezaevil81/Weblog-Laravel/actions/workflows/laravel.yml)
[![Laravel Version](https://img.shields.io/badge/Laravel-v12.x-FF2D20.svg)](https://laravel.com)
[![PHP Version](https://img.shields.io/badge/PHP-%3E%3D8.2-8892BF.svg)](https://www.php.net)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/alirezaevil81/Weblog-Laravel/blob/main/LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/alirezaevil81/Weblog-Laravel)](https://github.com/alirezaevil81/Weblog-Laravel/commits/main)

این پروژه یک سیستم وبلاگ ساده و مدرن است که با استفاده از جدیدترین ابزارهای اکوسیستم لاراول توسعه داده شده است. تمرکز اصلی این پروژه بر پیاده‌سازی یک سیستم احراز هویت امن و سفارشی، ساختاردهی تمیز قالب‌ها با Blade و راه‌اندازی یک فرآیند CI/CD خودکار با GitHub Actions بوده است.

---

## ✨ ویژگی‌های کلیدی و تکنولوژی‌ها

این پروژه برای نمایش مهارت در حوزه‌های زیر طراحی شده است:

- **Back-End:**
    - **Laravel 12:** استفاده از آخرین نسخه فریمورک و مفاهیم اصلی آن مانند مسیریابی (Routing)، کنترلرها و Eloquent ORM.
    - **سیستم احراز هویت یکپارچه:** پیاده‌سازی کامل فرآیندهای ثبت‌نام، ورود و خروج کاربران در یک کنترلر واحد (`AuthController`).
    - **اعتبارسنجی پیشرفته:** استفاده از Form Request (`LoginRequest`) برای جداسازی منطق اعتبارسنجی و افزایش امنیت.

- **Front-End:**
    - **Tailwind CSS 4:** طراحی کاملاً واکنش‌گرا و مدرن با بهره‌گیری از نسخه جدید و بهینه تیلوند.
    - **Vite:** مدیریت و کامپایل فوق‌العاده سریع فایل‌های CSS و JS.
    - **قالب‌بندی ماژولار با Blade:** جداسازی بخش‌های تکراری مانند هدر و فوتر با استفاده از `@include` برای خوانایی و مدیریت بهتر کد.

- **DevOps و تست:**
    - **GitHub Actions (CI):** راه‌اندازی یک ورک‌فلو خودکار برای اجرای تست‌های پروژه (PHPUnit) پس از هر `push`، جهت تضمین سلامت و پایداری کد.
    - **PHPUnit:** استفاده از تست‌های Feature و Unit برای اطمینان از عملکرد صحیح اپلیکیشن.

---

## 🚀 راه‌اندازی و نصب

برای اجرای این پروژه به صورت محلی، مراحل زیر را دنبال کنید.

### پیش‌نیازها

- PHP (نسخه 8.2 یا بالاتر)
- Composer
- Node.js و npm

### مراحل نصب

1.  **کلون کردن ریپازیتوری:**
    ```bash
    git clone [https://github.com/alirezaevil81/Weblog-Laravel.git](https://github.com/alirezaevil81/Weblog-Laravel.git)
    cd Weblog-Laravel
    ```

2.  **نصب وابستگی‌های PHP:**
    ```bash
    composer install
    ```

3.  **نصب وابستگی‌های Node.js:**
    ```bash
    npm install
    ```

4.  **راه‌اندازی فایل محیطی:**
    فایل `.env.example` را به `.env` کپی کرده و سپس کلید اپلیکیشن را تولید کنید.
    ```bash
    cp .env.example .env
    php artisan key:generate
    ```

5.  **اجرای پروژه:**
    در یک ترمینال، سرور Vite را اجرا کنید:
    ```bash
    npm run dev
    ```
    و در یک ترمینال دیگر، سرور لاراول را اجرا کنید:
    ```bash
    php artisan serve
    ```

حالا می‌توانید پروژه را در آدرس `http://127.0.0.1:8000` مشاهده کنید.

---

## 📄 لایسنس

این پروژه تحت لایسنس MIT منتشر شده است. برای اطلاعات بیشتر فایل `LICENSE` را مطالعه کنید.
