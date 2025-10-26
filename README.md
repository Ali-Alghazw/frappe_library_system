# Frappe Library System

A full Library Management System built using the Frappe Framework. It allows managing library members, books, and book transactions such as issuing and returning books.

## 🚀 Features

* Manage **Library Members** (create, view, edit, delete)
* Maintain **Book Catalog** with detailed information
* Issue & Return books with automatic date management
* Custom **Client Scripts & Hooks** integration
* Role-based permissions (Admin / Librarian)
* Built using **Frappe Framework** best practices

## 📦 Tech Stack

* **Python 3.x**
* **Frappe Framework**
* **MariaDB / MySQL**
* **Redis** (caching & queue)
* **Node.js & Yarn** (frontend build)

## 📁 Project Structure (important parts)

```
frappe_library_system/
 ├─ frappe_library_system/
 │   ├─ doctype/              # Custom doctypes
 │   ├─ hooks.py              # Client/Server scripts loader
 │   ├─ public/               # Static assets
 │   └─ README.md
 └─ ... (Frappe bench folders)
```

## 🛠️ Installation (Local Setup)

```bash
git clone https://github.com/Ali-Alghazw/frappe_library_system.git
cd frappe-bench
bench get-app ../frappe_library_system
bench --site site1.local install-app frappe_library_system
bench --site site1.local serve
```

Then visit: **[http://localhost:8000](http://localhost:8000)**

## 🔒 Default Login

```
Username: Administrator
Password: (the one you set during site creation)
```

## 📌 Usage

* Go to **Library > Library Members** to add members
* Go to **Library > Books** to manage books
* Use **Borrow / Return** Doctype to manage transactions

## ✅ Development Notes

* Client Scripts are loaded via `hooks.py`
* Use `bench --site site1.local clear-cache && bench build` after JS changes

## 🤝 Contributing

1. Fork the repo
2. Create a feature branch
3. Commit your changes
4. Open a pull request

## 📄 License

MIT — Free to use and modify.

---

Made by **Ali Al-Ghazw**
