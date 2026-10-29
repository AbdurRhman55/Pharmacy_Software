# 🏥 Pharmacy Software — Complete Management System

A modern, fast, and comprehensive Pharmacy Management and POS System designed for medical stores, pharmacies, and healthcare clinics.

---

## 🚀 Quick Start (cPanel / Hostinger / XAMPP / Localhost)

1. Upload the files to your web root (`public_html` or subdomain directory).
2. Open your browser and navigate to your domain/URL (e.g. `https://yourdomain.com`).
3. The **Setup Wizard** launches automatically on first run.
4. Complete the 4 simple setup steps:
   - **Store Details**: Name, Phone, NTN/STRN, Address, Currency (`Rs PKR`, `$ USD`, etc.)
   - **Admin Account**: Username, Email, and Secure Password
   - **Storage Engine**: Choose between **JSON File Storage** (zero-config, no DB setup required) or **MySQL**
   - **Confirm & Launch**: Review details and initialize
5. Log in with your admin credentials!

---

## 📋 Features Overview

### 1. Admin Portal
- **Dashboard**: Live real-time stats, 7-day revenue/sales chart, low stock alerts, near-expiry alerts, and quick actions.
- **Point of Sale (POS)**: Fast billing counter with barcode support, batch selector, live stock checking, instant invoice generation, and thermal/A4 receipt printing.
- **Medicine & Inventory Management**: Full CRUD, dosage forms, manufacturer, rack/shelf location, and bulk CSV import.
- **Batch & Expiry Tracking**: Track batches with manufacturing/expiry dates and automatic alert notifications.
- **Suppliers & Purchase Orders**: Manage suppliers, create POs, track received inventory, and auto-email orders.
- **Returns & Refunds**: Customer return management with stock restock handling.
- **Customer Directory**: Customer profiles, purchase history, and outstanding ledgers.
- **Financial Ledger & Analytics**: Income/expense statements, top selling medicines, payment breakdown, and monthly financial performance.
- **Role-based Access Control**: Manage Staff and Admin user accounts with restricted permissions.

### 2. Supplier Portal
- Dedicated supplier login and dashboard.
- View and manage purchase orders (Confirmed &rarr; Shipped &rarr; Received).
- Direct order confirmation and communication portal.

### 3. Customer / Patient Portal
- Patient account registration and login.
- Access purchase history and downloadable receipts/invoices.
- Submit return requests and inquiries.

---

## ⚙️ Requirements

- **PHP**: 7.4, 8.0, 8.1, 8.2, or 8.3
- **Extensions**: `pdo`, `pdo_mysql` (optional for MySQL mode), `json`, `session`, `mbstring`
- **Web Server**: Apache, Nginx, or LiteSpeed with `mod_rewrite` enabled
- **File Permissions**: Write permission on the `data/` directory (`chmod 755 data/`)

---

## 📁 Repository Structure

```
├── assets/             # CSS stylesheets, JavaScript files, and icons
├── config/             # Application configuration & system constants
├── data/               # Storage directory (JSON databases, schema, uploads)
├── docs/               # System documentation and user guides
├── helpers/            # Core helper classes (MySQLDB, JsonDB, Mailer, etc.)
├── public/
│   ├── admin/          # Admin POS and management controllers
│   ├── customer/       # Customer / Patient portal
│   ├── setup/          # Automated initial installation wizard
│   └── supplier/       # Supplier portal
├── views/              # Common UI templates and layouts
├── .htaccess           # Apache rewrite and security rules
├── index.php           # Front controller & application router
└── README.md
```

---

## 🛡️ Security Features

- **Password Hashing**: BCrypt encryption for user credentials.
- **CSRF Protection**: Token verification across all form submissions.
- **Brute Force Protection**: Automatic lockout after repeated failed login attempts.
- **XSS & SQL Injection Defense**: Prepared PDO queries and strict output sanitization.
- **Secure File Access**: Web access to internal data files blocked via `.htaccess`.

---

Developed & Maintained by **Abdur Rahman**
GitHub: [@AbdurRhman55](https://github.com/AbdurRhman55)
