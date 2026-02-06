# 🛒 Treabyn Global Mall (Headless Architecture)

![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![Role](https://img.shields.io/badge/Role-Full_Stack_Developer-blue?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-React_|_Google_Sheets_API_|_WhatsApp-green?style=for-the-badge)

## 📋 Executive Summary
A revolutionary "No-DB" e-commerce platform architected by **Adewole Felix Bamidele**. By utilizing **Google Sheets** as a relational database and **React** for the frontend, this project delivers enterprise-grade inventory management with **zero database hosting costs**.

## 🏗️ System Architecture

```mermaid
graph LR
    A[React Frontend] <-->|JSON Fetch| B(Google Sheets API v4)
    B <-->|Real-Time Sync| C[(Master Inventory Sheet)]
    A -->|State Mgmt| D{Redux Toolkit}
    D -->|Checkout Action| E[WhatsApp Business API]
    E -->|Order Details| F[Sales Agent Device]

    🛠️ Technical Know-How
1. The "Google Sheets as Backend" Strategy
API Wrapper: I built a custom adapter that fetches sheet data (Products, Categories, Prices) and converts it into a clean JSON object for the React frontend to consume.

Caching: Implemented localStorage caching to minimize API calls to Google, ensuring the site loads instantly even on slow 3G networks.

2. Direct-to-Agent Checkout
Instead of a generic payment gateway, the checkout button constructs a pre-filled WhatsApp URL containing the SKU, Quantity, and Total Price.

Result: This removes friction, allowing customers to negotiate and confirm orders directly with a human agent in real-time.

3. Responsive Component Design
Built with a Mobile-First grid using Tailwind CSS, ensuring the "Product Cards" and "Cart Drawer" perform natively on Android and iOS devices.

Architected by: Adewole Felix Bamidele Master's Degree (2015) | Solutions Architect