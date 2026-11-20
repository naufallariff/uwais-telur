# 🥚 Uwais Telur — Point of Sale & Distribution Management System

**A lightweight, offline-first web-based POS, inventory, and transaction management system tailored for wholesale and retail egg distribution.**

[Overview](https://www.google.com/search?q=%23-overview) • [Key Features](https://www.google.com/search?q=%23-key-features) • [Tech Stack](https://www.google.com/search?q=%23-tech-stack) • [Architecture](https://www.google.com/search?q=%23-architecture) • [Getting Started](https://www.google.com/search?q=%23-getting-started) • [Publication](https://www.google.com/search?q=%23-research--publication)

---

## 📖 Overview

**Uwais Telur POS** is a custom-built web application designed to streamline daily operations for egg distribution businesses. Legacy retail POS tools often suffer from bloated, irrelevant features, unintuitive payment tracking, and rigid data lock-in.

Built on a clean **Model-View-Controller (MVC)** architecture, this system runs locally without requiring an active internet connection—ensuring zero-latency operations at the storefront while maintaining strict transactional integrity across sales, supplier procurement, stock levels, and installment payments.

---

## ✨ Key Features

* 🛒 **Sales & Multi-Item Order Processing**
Create itemized sales orders rapidly with dynamic search (`Select2`), automatic subtotal calculations, and inline customer registration without leaving the transaction workflow.
* 💳 **Real-Time Payment & Debt Monitoring**
Supports both full and partial (installment) payments for customer receivables and supplier payables, complete with color-coded status indicators (`Lunas` / `Belum Lunas`) and payment history logs.
* 📦 **Automated Inventory Synchronization**
Stock quantities automatically adjust in real time whenever sales orders or supplier purchase transactions are recorded, updated, or voided.
* 📊 **One-Click Excel Data Backup**
Export transaction records directly into `.xlsx` spreadsheets for independent financial reporting, external auditing, and offline data redundancy.
* 🖨️ **Configurable Receipt Printing**
Built-in thermal/invoice receipt generation driven by a modular hardware configuration (`printer-config.json`).
* 🔐 **Secure Admin Authentication & Middleware**
Session-based access control, request logging, and centralized error handling to safeguard operational records.

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
| --- | --- | --- |
| **Runtime** | Node.js | Server-side JavaScript execution environment |
| **Backend Framework** | Express.js | RESTful routing, middleware pipeline, and server logic |
| **Templating Engine** | EJS | Server-side dynamic HTML rendering |
| **Database Engine** | SQLite | Lightweight, serverless embedded relational storage |
| **Frontend UI** | HTML5, CSS3, jQuery, Select2 | Responsive dashboard layout and searchable dropdown controls |
| **Code Quality & CI** | ESLint, GitHub Actions | Automated linting and continuous integration checks |

---

## 🏗️ Architecture

The application follows a decoupled **MVC (Model-View-Controller)** pattern separating business logic, data persistence, and presentation layers. For security and data privacy, database schemas and internal storage structures are abstracted behind dedicated model layers.

---

## 🚀 Getting Started

### Prerequisites

* **Node.js** (v18.x or higher recommended)
* **npm** (comes bundled with Node.js)

### Installation & Local Setup

1. **Clone the repository**
```bash
git clone https://github.com/your-username/uwais-telur.git
cd uwais-telur

```


2. **Install dependencies**
```bash
npm install

```


3. **Configure environment & hardware**
* Review `config/config.js` to adjust application ports or session secrets as needed.
* Update `config/printer-config.json` to match your local receipt printer setup.


4. **Start the application**
```bash
npm start

```


5. **Access the dashboard**
Open your browser and navigate to `http://localhost:3000` (or your configured port).

---

## 📄 Research & Publication

The engineering methodology, requirements analysis, and system evaluation behind this project have been peer-reviewed and published in **The Indonesian Journal of Computer Science (IJCS)**:

> **Pengembangan Sistem Transaksi Penjualan Toko Uwais Telur Menggunakan Metode Rapid Application Development**
> *Muhammad Naufal Arif, Amalia, Misna Asqia*
> 🔗 **DOI:** [https://doi.org/10.33022/ijcs.v14i5.4961](https://doi.org/10.33022/ijcs.v14i5.4961)
> 🌐 **Article URL:** [https://www.ijcs.net/ijcs/index.php/ijcs/article/view/4961](https://www.ijcs.net/ijcs/index.php/ijcs/article/view/4961)

---

## 👨‍💻 Author & License

* **Developer:** Muhammad Naufal Arif
* **License:** Licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).
