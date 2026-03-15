
# 💰 Finance Manager

A secure, responsive personal expense and income management system built with PHP and MySQL.

![PHP](https://img.shields.io/badge/PHP-8.2+-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-5.7+-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3.0-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)

## ✨ Features

- **📊 Visual Dashboard** — Interactive charts with Chart.js showing income vs expenses, spending breakdowns, and monthly trends
- **💳 Transaction Management** — Track income and expenses with categories, descriptions, and receipt uploads
- **📅 Recurring Transactions** — Set up daily, weekly, monthly, or yearly recurring entries
- **🎯 Budget Planning** — Category-based budgets with spending alerts and visual progress bars
- **🔍 Advanced Filtering** — Search, filter by date range, category, payment method, and amount
- **📤 Data Export** — Export transactions to CSV with one click
- **📱 Responsive Design** — Works seamlessly on desktop, tablet, and mobile
- **🔐 Security First** — CSRF protection, prepared statements, password hashing, and session security

## 🚀 Quick Start

### Requirements
- PHP 8.2+
- MySQL 5.7+ or MariaDB 10.3+
- Apache/Nginx with mod_rewrite
- SSL certificate (recommended for production)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/finance-manager.git
   cd finance-manager

2.  **Create the database**
    
    -   Import `database.sql` into your MySQL server
        
    -   This creates all tables and default categories
        
3.  **Configure database connection**
    
    -   Copy `includes/config.php` and update with your credentials:
        
    
    php

    
    ```php
    define('DB_HOST', 'localhost');
    define('DB_USER', 'your_username');
    define('DB_PASS', 'your_password');
    define('DB_NAME', 'your_database');
    ```
    
4.  **Set up uploads folder**
   
    
    ```bash
    mkdir uploads
    chmod 755 uploads
    ```
    
5.  **Access the application**
    
    -   Navigate to `https://yourdomain.com/`
        
    -   First-time setup will prompt you to create an admin account
        

## 📁 Project Structure

```plain
finance-manager/
├── index.php              # Login & setup
├── dashboard.php          # Main dashboard with charts
├── transactions.php       # Transaction list with filters
├── transaction-form.php   # Add/edit transactions
├── delete-transaction.php # Delete handler
├── reports.php            # Analytics & reports
├── budgets.php            # Budget management
├── settings.php           # User settings
├── export-csv.php         # CSV export
├── logout.php             # Logout handler
├── database.sql           # Database schema
├── includes/
│   ├── config.php         # Database configuration
│   ├── functions.php      # Helper functions
│   ├── auth-check.php     # Authentication
│   ├── header.php         # Common header
│   └── footer.php         # Common footer
├── uploads/               # Receipt storage
└── README.md
```

## 🛡️ Security Features

-   ✅ **PDO Prepared Statements** — SQL injection protection
    
-   ✅ **Password Hashing** — Bcrypt with secure defaults
    
-   ✅ **CSRF Tokens** — All forms protected
    
-   ✅ **XSS Prevention** — Output escaping with `htmlspecialchars()`
    
-   ✅ **Session Security** — HttpOnly, Secure, SameSite cookies
    
-   ✅ **File Upload Validation** — MIME type and size checking
    

## 🎨 Screenshots

ADDING SOON


## 🛠️ Customization

### Default Categories

**Income:** Salary, Freelance, Investments, Gifts Received, Other Income

**Expenses:** Food & Dining, Transportation, Housing & Rent, Utilities, Entertainment, Healthcare, Shopping, Education, Travel, Subscriptions, Personal Care, Gifts Given, Other Expense

Modify categories directly in the database or add new ones via SQL.

### Currency Support

Built-in support for: USD, EUR, GBP, INR, JPY, CAD, AUD, CHF, CNY, BRL


## 🙏 Credits

-   [Tailwind CSS](https://tailwindcss.com/) — Utility-first CSS framework
    
-   [Chart.js](https://www.chartjs.org/) — JavaScript charting
    
-   [Lucide Icons](https://lucide.dev/) — Beautiful icons
    

----------

**Happy budgeting!** 💸
---

If you want, I can also create:

1. **DEPLOYMENT.md** — Detailed Hostinger deployment guide
2. **LICENSE** — MIT license file
3. **.htaccess** — Security configuration for Apache
4. **CONTRIBUTING.md** — Contribution guidelines

Would you like me to generate any of these additional files