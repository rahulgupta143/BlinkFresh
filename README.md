# ⚡ BlinkFresh

### Hyperlocal 6-Minute APMC Mandi & Grocery Delivery Web Application

**Freshness at Your Doorstep. Mandi Prices. Smarter Shopping.**

BlinkFresh is a hyperlocal grocery delivery web application designed to connect households with local APMC mandi suppliers and nearby micro-dark stores. It provides fresh vegetables, fruits, daily essentials, weight-based pricing, and a modern shopping experience.

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Tech Stack](#️-tech-stack)
- [Repository Structure](#-repository-structure)
- [Quick Start](#-quick-start)
- [Mobile Responsiveness](#-mobile-responsiveness)
- [Future Roadmap](#-future-roadmap)
- [License](#-license)

## 🚀 Project Overview

BlinkFresh combines the convenience of quick-commerce platforms with the affordability and freshness of local vegetable markets.

The application follows a zero-bundler, single-file architecture, allowing the standalone HTML version to run directly in a modern browser without requiring Node.js, npm, or a build process.

### Core Objectives

- Fresh vegetables, fruits, and grocery essentials.
- Flexible weight-based product pricing.
- Fast and intuitive shopping cart.
- Interactive delivery tracking interface.
- Online UPI QR and Cash on Delivery options.
- Family and flatmate bill splitting.
- English, Hindi, and Marathi language support.

## ✨ Key Features

### 1. ⚖️ Dynamic Weight-Based Pricing

- Select `250g`, `500g`, `1kg`, `2kg`, or `5kg`.
- Automatic price calculation.
- Product discounts and inventory indicators.
- Multiple weight variants of the same product in one cart.

### 2. 📝 Mummy Ki Parchi — Smart Grocery List

Convert grocery notes into shopping cart items.

**Example:**

```text
1kg aloo
500g tamatar
2 bread
1L milk
```

Features:

- Automatic quantity and weight extraction.
- Regional aliases such as aloo, batata, pyaaz, kanda, and tamatar.
- Bulk-add functionality.
- Itemized confirmation before checkout.

### 3. 🗺️ Interactive GPS Delivery Tracking

- Leaflet.js interactive map.
- OpenStreetMap-compatible geographic data.
- CartoDB Voyager map tiles.
- Delivery hub and customer markers.
- Route visualization and animated rider marker.
- Delivery verification PIN interface.

*Real-time GPS tracking requires location permissions and a suitable backend or tracking service.*

### 4. 👥 Family & Flatmate Bill Split

- Group-based bill sharing.
- Equal per-person cost calculation.
- Itemized grocery bill.
- WhatsApp-ready bill summary.

### 5. 🥛 Morning Milk & Breakfast Subscriptions

- Daily delivery.
- Alternate-day delivery.
- Weekday delivery (Monday–Friday).
- Milk, bread, eggs, and other breakfast essentials.
- Subscription delivery-fee indicators.

### 6. 🌿 Dhaniya-Mirchi Freebie Engine

- Unlock free coriander and green chillies (50g) at ₹149 in fresh produce.
- Visual cart milestone tracker.
- Automatic calculation of the remaining amount required.

### 7. 💳 Dual Payment Options

**UPI QR Payment**

- SVG-based QR display.
- Payment amount presentation.
- Copyable UPI details.
- Payment status interface.

UPI ID: `blinkfresh.mandi@icici`

**Cash on Delivery (COD)**

- Pay at the doorstep.
- Cash payment instructions.
- Change advisory indicators.

*Real payment processing requires a payment gateway and server-side payment verification.*

### 8. 🌐 Trilingual Localization

Available languages:

- English
- हिन्दी
- मराठी

The interface supports translated product names, categories, promotional labels, and system messages.

### 9. 🎁 Mystery Scratch Card & BlinkCash

- Interactive scratch-card experience.
- Reward concept ranging from ₹15 to ₹50.
- BlinkCash wallet integration concept.
- Celebration animations and sound effects.

*Secure reward credits require backend validation and persistent storage.*

### 10. 🎙️ Voice Search & Interactive Feedback

- Browser-based speech recognition where supported.
- Voice-assisted product search.
- Web Audio API sound effects.
- Mobile vibration feedback on supported devices.
- Interactive UI animations.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and animations |
| JavaScript | Application logic |
| Tailwind CSS CDN | Utility-based styling |
| Leaflet.js 1.9.4 | Interactive maps |
| CartoDB Voyager | Map styling |
| OpenStreetMap | Geographic map data |
| Lucide Icons | Interface icons |
| Unsplash CDN | Product imagery |
| Web Audio API | Sound effects |
| Canvas Confetti | Celebration animations |
| Web Speech API | Voice search |
| Browser Storage | Optional local persistence |

## 📁 Repository Structure

```text
blinkfresh/
├── index.html
│   └── Complete standalone web application
├── App.jsx
│   └── React component alternative
├── project_description.md
│   └── Project specifications
└── README.md
    └── Project documentation
```

## ⚡ Quick Start

### Prerequisites

- A modern web browser.
- Internet connection for external CDN libraries, maps, and images.

No Node.js, npm, or build tools are required to run the standalone HTML version.

### Option 1: Direct Browser Run

**Step 1:** Clone the repository.

```bash
git clone https://github.com/your-username/blinkfresh.git
```

**Step 2:** Open the project directory.

```bash
cd blinkfresh
```

**Step 3:** Open `index.html` in your browser.

Replace `your-username` with your actual GitHub username.

### Option 2: Python HTTP Server

Run:

```bash
python -m http.server 3000
```

Open:

```text
http://localhost:3000
```

### Option 3: Node.js

Run:

```bash
npx serve .
```

Open the local URL displayed in your terminal.

## 📱 Mobile Responsiveness

BlinkFresh uses a mobile-first design approach.

- Touch-friendly controls.
- Responsive product cards.
- Mobile-friendly address and delivery indicators.
- Floating cart shortcut.
- Compact checkout experience.
- Optional vibration feedback on supported devices.

## 🔮 Future Roadmap

- [ ] User registration and secure authentication.
- [ ] MongoDB database integration.
- [ ] Persistent cart and order history.
- [ ] Live inventory management.
- [ ] Admin dashboard.
- [ ] Real UPI payment gateway.
- [ ] Server-side payment verification.
- [ ] Live delivery partner GPS tracking.
- [ ] Delivery radius and estimated delivery calculation.
- [ ] Automated subscription scheduling.
- [ ] Secure BlinkCash wallet.
- [ ] Progressive Web App (PWA) support.
- [ ] Order notifications and customer support.

**Delivery promise:** The 6-minute target depends on product availability, customer distance, rider availability, and local operating conditions.

## 🔐 Security & Production Readiness

Before launching BlinkFresh for real customers:

- Keep database credentials and API secrets on the server.
- Validate product prices, quantities, and discounts server-side.
- Verify payments through trusted payment-provider webhooks.
- Implement secure authentication and authorization.
- Validate delivery addresses and service areas.
- Protect customer information and order records.
- Never treat frontend animations as proof of payment.

The standalone HTML version is suitable for prototypes and demonstrations. A production multi-user platform requires a secure backend and persistent database.

## 📄 License

This project is intended to use the **MIT License**.

Include the appropriate MIT license text in a `LICENSE` file before distributing the project under that license.

## 👨‍💻 Author

**Rahul Gupta**

- GitHub: [@rahulgupta143](https://github.com/rahulgupta143)
- Project: BlinkFresh

---

### ⚡ BlinkFresh

**Fresh Mandi Products. Smarter Prices. Faster Shopping.**

*Bringing the local mandi closer to your home.*
