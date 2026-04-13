# 🛍️ VOGUE STORE — Django E-Commerce Website

A full-featured fashion e-commerce web application built with **Python + Django**, featuring a premium black & gold UI design for Men's, Women's, and Kids' clothing.

---

## 🌟 Features

- 🏠 **Home Page** — Hero carousel, category sections (Men / Women / Kids), product grid
- 🛍️ **Product Listing** — Search by name, filter by category, product cards with hover actions
- 🛒 **Shopping Cart** — Add/remove items, increase/decrease quantity, grand total
- ❤️ **Wishlist** — Save products, move to cart, remove items
- 📦 **Checkout** — Full address form, payment method selection (COD / UPI / Card)
- 📋 **Order History** — View all past orders per user
- 👤 **Authentication** — Register, Login, Logout with session management
- 📧 **Email Confirmation** — Sends order confirmation on successful purchase
- 🔧 **Admin Dashboard** — Manage products, orders, users, contacts with search & filters

---

## 🖥️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python 3.12, Django 5.2 |
| Database | SQLite (development) |
| Frontend | HTML5, CSS3, Bootstrap 5.3 |
| Fonts | Google Fonts (Playfair Display + Inter) |
| Icons | Font Awesome 6 |
| Auth | Django built-in Auth |

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/vogue-store.git
cd vogue-store
```

### 2. Create Virtual Environment
```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install django pillow
```

### 4. Set Up Environment Variables (optional — for email)
Create a `.env` file:
```
EMAIL_HOST_USER=your@gmail.com
EMAIL_HOST_PASSWORD=your_app_password
```

### 5. Run Migrations
```bash
python manage.py migrate
```

### 6. Create Superuser (Admin)
```bash
python manage.py createsuperuser
```

### 7. Run the Server
```bash
python manage.py runserver
```

Visit → **http://127.0.0.1:8000/**

---

## 📁 Project Structure

```
EStore/
├── EStore/                 # Django project settings
│   ├── settings.py
│   └── urls.py
├── store/                  # Main app
│   ├── models.py           # Product, Cart, Order, Wishlist, Contact, Rating
│   ├── views.py            # All view logic
│   ├── urls.py             # URL routing
│   └── admin.py            # Admin customization
├── templates/              # HTML templates
│   ├── base.html           # Shared navbar + footer
│   ├── index.html          # Homepage
│   ├── product_list.html   # Product listing + search
│   ├── product_cart.html   # Shopping cart
│   ├── checkout.html       # Checkout form
│   ├── order_history.html  # Order history
│   ├── wishlist.html       # Wishlist page
│   ├── success.html        # Order success
│   ├── about.html
│   ├── contact.html
│   └── registration/
│       ├── login.html
│       └── register.html
├── static/                 # CSS, JS, images
├── media/                  # Uploaded product images
└── manage.py
```

---

## 📷 Pages Overview

| Page | URL |
|------|-----|
| Home | `/` |
| All Products | `/product-list/` |
| Men's | `/product-list/?category=men` |
| Women's | `/product-list/?category=women` |
| Kids' | `/product-list/?category=kids` |
| Cart | `/product-cart/` |
| Checkout | `/checkout/<id>/` |
| Order History | `/order-history/` |
| Wishlist | `/wishlist/` |
| Admin | `/admin/` |
| Register | `/register/` |
| Login | `/login/` |

---

## 🔐 Admin Access

Visit `/admin/` and log in with your superuser credentials.

From the admin panel you can:
- Add / edit / delete products
- View all orders
- See customer messages (Contact form)
- Manage users, wishlists, carts

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

## 📄 License

MIT License — free to use for personal & commercial projects.

---

*Built with ❤️ using Django — VOGUE STORE*
