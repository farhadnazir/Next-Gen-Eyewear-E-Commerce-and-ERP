# 👓 Next-Gen Eyewear E-Commerce & ERP

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![Livewire](https://img.shields.io/badge/Livewire-4E56A6?style=for-the-badge&logo=livewire&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

Next-Gen Eyewear  is a bespoke, enterprise-grade E-commerce and Inventory Management System engineered specifically for the optical industry. It seamlessly bridges the gap between complex optical prescriptions (frames, contact lenses, Rx) and a modern, high-converting retail experience.

Built with performance and scalability in mind, it replaces traditional disjointed tools with a unified platform for inventory sync, financial analytics, and customer relationship management.

---

## ✨ Highlighted Features

### 🛍️ Smart Optics Catalog & Cart
* **Complex Product Typology:** Distinct engines for Standard Frames, Sunglasses, and Contact Lenses.
* **The Lens Engine:** Handles dynamic optical parameters (SPH, SPH-CYL, Base Curve, Diameter) natively within the cart.
* **Volume Pricing:** Automated tier-based discounts for contact lenses (e.g., "Buy 4+ Boxes, Save 10%").
* **Advanced Filtering:** Filter catalog by face shape, frame material, gender, and color variants.

### 📦 Intelligent Inventory & ERP
* **Variant-Level Syncing:** Real-time stock deduction on checkout and automated restocking on order cancellation.
* **Low Stock Alerts:** Smart dashboard widget that detects low inventory across base products AND specific color/size variants.
* **Prescription (Rx) Vault:** Customers can upload or manually input optical prescriptions, securely saved to their profile.

### 📊 Financial Intelligence & Moderation
* **Admin Command Center:** Real-time analytics, MoM (Month-over-Month) revenue growth, and active order tracking.
* **Verified Review Engine:** Strict "Buyers Only" review policy with a moderation queue (Approve/Reject) and dynamic star-rating distribution charts.
* **Automated Invoicing:** Auto-generated PDF receipts upon order completion.

---

## 💻 Tech Stack & Development Journey

**Development Timeline:** Architected and deployed within a rapid, focused development cycle.
**Core Philosophy:** SPAs (Single Page Applications) feel without the overhead of a separate JS framework, achieved through Livewire.

* **Backend Framework:** Laravel 11/12
* **Frontend Reactive Engine:** Livewire 3
* **Styling & UI:** Tailwind CSS, FontAwesome, Alpine.js
* **Database:** MySQL (Relational architecture for complex variants)
* **Authentication:** Laravel Breeze

---



## 📸 Platform Gallery

| Customer View |
|:---:|
| <video src="https://github.com/user-attachments/assets/ee7cd333-716a-4c4d-b475-13e6ec0757de" width="400">|
| Admin Command Center |
|:---:|
| <video src="https://github.com/user-attachments/assets/06a015f5-d47e-475d-8848-d0a578f83a58" width="400" alt="Dashboard"> |
| **Contact Lens Engine** |
| <video src="https://github.com/user-attachments/assets/7459287c-3b2d-4fb1-b8d7-f833fd4d9887" width="400" alt="Lens Engine"> |

*(Replace the placeholder URLs above with actual screenshots of your application)*

---

## 🗄️ Core Database Schema

The architecture is highly relational to support the optical business logic:

* `users`: Core authentication and role management (Admin/Customer).
* `products`: Base product information, type (Frame/Lens), and base pricing.
* `product_variants`: Handles colors, size categories, and variant-specific stock levels.
* `contact_lens_details`: specialized table for SPH limits, BC, DIA, and JSON volume pricing.
* `orders` & `order_items`: Financial transactions and cart history.
* `product_reviews`: Verified buyer ratings, linked to `users` and `products` with status toggles.

---

## 📂 Project Architecture (Livewire Approach)

The application relies heavily on component-based architecture for real-time reactivity without page reloads:

```text
app/Livewire/
├── Admin/
│   ├── Dashboard.php              # Analytics & Low Stock Logic
│   ├── ProductManager.php         # Base CRUD
│   ├── ProductVariantManager.php  # Variant Engine
│   ├── ContactLensManager.php     # Rx & Volume Configurator
│   └── ReviewManagement.php       # Moderation Queue
└── Frontend/
    ├── ProductCatalog.php         # Advanced Filtering
    ├── ContactLensShopper.php     # Rx Input & Tiered Pricing Cart
    ├── CheckoutPage.php           # Secure Checkout & Stock Deduct
    └── ProductReviews.php         # Star Distribution & Submission
```

🛡️ License & Contact
This project is proprietary. Developed as a comprehensive solution for the optical retail sector.

Developed by: [Farhad Nazir]

Role: Full Stack Developer (Laravel / Flutter)

Connect on linkedin: [https://www.linkedin.com/in/farhadnazir]
