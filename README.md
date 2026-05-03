# 🔄 Swapify — Cozy Community Marketplace

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Swapify is a full-featured web application that enables community-driven swapping of skills, physical items, and half-price deals. The platform focuses on reducing waste, building local connections, and fostering a trust-based sharing economy.

---

## 📸 Visual Preview

### 🖥️ Core Interfaces
Experience a cozy and intuitive community environment across all devices.

| Login Interface | Main Community Page | User Profile |
| :---: | :---: | :---: |
| ![Login](screenshots/login.png) | ![Main Page](screenshots/main_page.png) | ![Profile](screenshots/profile.png) |
| *Interactive Lamp Toggle UI* | *Skill & Object Swap Feed* | *Manage Wallet & Swaps* |

---

### 🛍️ Marketplace & Shopping
A seamless flow from discovering deals to secure simulated checkout.

| Half-Price Deals | Shopping Cart | Secure Payment |
| :---: | :---: | :---: |
| ![Deals](screenshots/half_price_deals.png) | ![Cart](screenshots/cart.png) | ![Payment](screenshots/payment.png) |
| *Daily Point-Redeemable Deals* | *Persistent LocalStorage Cart* | *Points & Promo Integration* |

---

### 📖 User Onboarding & Communication
<details>
<summary><b>Click to view Onboarding and Messaging Flow</b></summary>

#### Onboarding Experience
A 3-stage welcome flow to set up user preferences and community location.
<p align="center">
  <img src="screenshots/welcome1.png" width="30%" alt="Welcome 1">
  <img src="screenshots/welcome2.png" width="30%" alt="Welcome 2">
  <img src="screenshots/welcome3.png" width="30%" alt="Welcome 3">
</p>

#### Real-time Messaging
Connect with swappers instantly via the built-in chat interface.
<p align="center">
  <img src="screenshots/messages.png" width="80%" alt="Chat Interface">
</p>

</details>

---

## 🌟 Overview

**Swapify** allows users to:
*   Swap **skills** (teach photography, get guitar lessons, etc.).
*   Swap **physical objects** (furniture, electronics, clothing).
*   Buy/sell **half-price deals** with a points-based rewards system.
*   Earn **Swapify Points** on purchases and redeem them for discounts.
*   Report users and manage community safety.

Built with vanilla HTML/CSS/JS, the app uses `localStorage` as its data store, making it fully client-side and ready to run without a backend server.

---

## ✨ Features

### Core Marketplace
*   **Skill Swaps**: Offer and request skills with level ratings (Beginner → Expert).
*   **Object Swaps**: Trade physical items; each listing shows "wants".
*   **Half-Price Deals**: Discounted items with cart, checkout, and payment simulation.
*   **Search & Filters**: Live search + multi-criteria filtering (category, condition, rating, level, location).
*   **Favorites**: Heart-based wishlist system[cite: 1].

### Shopping & Rewards
*   **Shopping Cart**: Persistent cart with quantity controls and stock management.
*   **Checkout**: Credit/debit card form, Cash on Delivery, and 50% split payment plan options.
*   **Swapify Points**: Earn 10 points per $1 spent; 100 points = $1 discount.
*   **Wallet**: View points balance, transaction history, and saved payment cards.

### Communication & Safety
*   **Messaging**: Real-time chat between users with message status (sent/delivered).
*   **Reporting**: Comprehensive user/listing report form with file attachments (images/PDF).

### Admin Dashboard
*   **User Management**: View, search, ban, suspend, activate, or delete users.
*   **Skill Moderation**: Approve or reject skill listings.
*   **Metrics**: Live stats (users, skills, swaps, open reports).
---

## 🛠️ Technology Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend** | HTML5, CSS3, JavaScript (ES6+)[cite: 1] |
| **Animation** | CSS keyframes + GSAP (for lamp toggle effect on login page)[cite: 1] |
| **Storage** | `localStorage` (client-side persistence)[cite: 1] |
| **Architecture** | Modular global objects (`SwapifyAuth`, `SwapifyStore`, etc.)[cite: 1] |

---

## 🚀 Getting Started

### Prerequisites
*   Any modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)[cite: 1].
*   No server, database, or build step required[cite: 1].

### Installation
1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/yourusername/swapify.git](https://github.com/yourusername/swapify.git)
    cd swapify
    ```
2.  **Open `index.html`** directly in your browser[cite: 1].

### Default Test Accounts
| Role | Email | Password |
| :--- | :--- | :--- |
| **Admin** | `sarah@example.com` | `Test@1234` |
| **User** | `carlos@example.com` | `Test@1234` |

**Admin PIN**: `2580`[cite: 1].

---

## 💾 Data Persistence

All data is stored in `localStorage` under the `swapify_` prefix[cite: 1]:

*   `swapify_users`: User accounts and profiles[cite: 1].
*   `swapify_skills`: Skill listings[cite: 1].
*   `swapify_messages`: Chat history[cite: 1].
*   `swapify_cart_{userId}`: User-scoped shopping cart[cite: 1].

---
