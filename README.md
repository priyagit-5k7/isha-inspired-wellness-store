# Root & Ritual — Isha-Inspired Indian Lifestyle Storefront

[![Vite](https://img.shields.io/badge/Vite-8.3.4-646CFF?style=flat&logo=vite)](https://vite.dev)
[![React](https://img.shields.io/badge/React-19.3.1-61DAFB?style=flat&logo=react)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?style=flat&logo=typescript)](https://www.typescriptlang.org)
[![Tests](https://img.shields.io/badge/Vitest-10%2F10%20Passing-brightgreen?style=flat&logo=vitest)](https://vitest.dev)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Important Student Concept Disclosure:** This website is an **independent student concept and portfolio tribute**, inspired by the serene architecture, consecrated spaces, and mindful lifestyle ethos of the Isha Yoga Center in Coimbatore, Tamil Nadu. It is **not** an official Isha Foundation website, nor is it endorsed by, affiliated with, or operated by Isha Foundation or Sadhguru. All product offerings, prices, ratings, and quotes are realistic fictional representations curated for educational design demonstration. No actual transactions are processed.

---

## 🌿 Final Enhanced Highlights & Temple-Inspired Experience

### 1. Isha-Inspired Visual Identity & Architecture
- **Aesthetic Direction:** Warm ivory backgrounds (`#FAF7F2`), deep forest green (`#2D4030`), earthy brown (`#6E5D4F`), and muted gold accents (`#C29B38`) with typography combining classical serif (`Cinzel` & `Playfair Display`) and modern sans-serif (`Inter`).
- **Brand Wordmark & Emblem:** Stylized sacred flame and consecrated lotus emblem accompanying `ROOT & RITUAL`.
- **Top Announcement Strip:** Highlighting the independent concept tribute on every route.

### 2. 7-Slide Automatic Hero Gallery
The homepage features an automatic, pause-on-hover, touch-swipable 7-slide hero showcase highlighting consecrated temple spaces, Dhyanalinga architecture, and green foothills:
1. **Slide 1 — Find a Moment of Stillness:** Consecrated water bodies and Isha Yoga Center natural surroundings (`https://images.locationscout.net/2024/07/isha-foundation-india-8dto.jpg?w=1080&q=60`).
2. **Slide 2 — Explore Spaces for Meditation:** Dhyanalinga dome and consecrated meditation spaces (`https://static.sadhguru.org/d/46272/1748083560-image-2.jpg`).
3. **Slide 3 — Sacred Feminine Consecration:** Linga Bhairavi shrine with traditional oil lamps (`https://static.sadhguru.org/d/46272/1703141040-lingabhairavi-isha-yoga-center-coimbatore.jpg`).
4. **Slide 4 — Classical Sadhana Attire:** Practitioners in quiet natural surroundings with unbleached organic handlooms.
5. **Slide 5 — Timeless Temple Architecture:** Carved Dravidian stone pillars and lotus water tanks.
6. **Slide 6 — Living in Harmony with Nature:** Native agricultural harvests, organic unpolished grains, and eco-living.
7. **Slide 7 — Fragrance of Devotion:** Temple-grade sandalwood agarbatti and sacred altar accessories.
- **Controls & Accessibility:** Previous & Next arrow buttons, interactive slide indicators, play/pause toggle, keyboard arrow navigation, visibility-aware pausing, and resilient fallback images.

### 3. "Explore Yoga & Meditation" Horizontal Carousel
Immediately below the hero gallery, a dedicated horizontal carousel presents 7 image cards:
- *Classical Yoga (Hatha & Asana Sadhana)*
- *Meditation Spaces (Inner Silence & Buckwheat Cushions)*
- *Inner Stillness (Sadhana & Breath with Copper Vessels)*
- *Sacred Spaces (Altar & Consecrated Bell-Metal Brass)*
- *Mindful Living (Earthen Terracotta & Nature)*
- *Purity & Fragrance (Sandalwood & Cold-Pressed Cleansers)*
- *Conscious Nutrition (Native Millets & Flours)*
Equipped with previous/next navigation buttons, smooth scroll-snapping, and touch-swipe compatibility.

### 4. Traditional Quote Panel on Every Route
A reusable [`TraditionalQuotePanel`](file:///C:/Users/PriyaDharshini%20R/OneDrive/Desktop/isha_ui/src/components/ui/TraditionalQuotePanel.tsx) is rendered near the footer across all routes (`/`, `/shop`, `/product/:slug`, `/cart`, `/checkout`, `/order-confirmation`):
- Finished with ornamental Indian corner accents (`✦`), fine gold borders, a central consecrated lotus medallion, and verified yogic reflections.

### 5. Preserved & Expanded Shopping Features
- **6 Categories:** Traditional Clothing, Accessories & Ornaments, Food and Daily Essentials, Food Powders, Home & Living, and Wellness & Herbal Care.
- **Product Details:** Active multi-image thumbnails, tabbed accordion (Description, How to Use, Ingredients & Dimensions, Care & Safety, Sample Customer Reviews), sequential Previous/Next product navigation, and frequently paired bundles.
- **Header Actions:** Single horizontal desktop navbar, expandable search bar with instant autocomplete suggestions, wishlist counter, and cart indicator.
- **Interactive Modals:** Quick-View product modal, animated mobile navigation drawer, and responsive slide-out shop filter drawer.
- **Checkout & Confirmation:** Complete simulated form validation for Indian addresses and PIN codes with zero payment collection.

---

## 🛠️ Tech Stack & Architecture

- **Framework:** React 19 + TypeScript 5.8
- **Tooling:** Vite 8.3
- **Navigation:** React Router DOM 7
- **Icons:** Lucide React
- **Testing:** Vitest + React Testing Library + jsdom
- **State & Storage:** React Context (`CartContext`, `WishlistContext`, `ToastContext`) + LocalStorage
- **Deployment Configuration:** `vercel.json` SPA rewrite rule

---

## 🚀 Getting Started

### Installation & Setup

1. **Clone or enter the project directory:**
   ```bash
   cd isha_ui
   ```

2. **Install project dependencies:**
   ```bash
   npm install
   ```

3. **Start local development server:**
   ```bash
   npm run dev
   ```
   Open `http://localhost:5173` in your browser.

4. **Run Automated Test Suite (10/10 Passing):**
   ```bash
   npm test
   ```

5. **Build for Production Deployment:**
   ```bash
   npm run build
   ```
   Generates production bundle in `dist/`.

---

## 🧪 Acceptance Test Scenarios (TC01–TC10)

| Test ID | Description | Result |
|---|---|---|
| **TC01** | Homepage loads with hero slideshow, yoga gallery, and product sections | **PASS** |
| **TC02** | Search filters and displays matching products | **PASS** |
| **TC03** | Product can be added to cart and persists in `localStorage` | **PASS** |
| **TC04** | Increasing line item quantity updates totals dynamically | **PASS** |
| **TC05** | Invalid quantities are rejected (bounded by stock and min 1) | **PASS** |
| **TC06** | Out-of-stock items disable purchase buttons | **PASS** |
| **TC07** | Submitting invalid checkout fields triggers accessible validation errors | **PASS** |
| **TC08** | Valid checkout simulation completes, generates mock order, and clears cart | **PASS** |
| **TC09** | Admin stock scenario is verified as intentionally **Out of Scope** | **PASS** |
| **TC10** | Mobile drawer and responsive filter controls remain accessible | **PASS** |

---

## 🌐 Public Deployment Instructions

The project is structured for deployment on Vercel, Netlify, or any static hosting provider:

### Vercel Deployment
1. Import the repository into [Vercel](https://vercel.com).
2. Framework Preset: **Vite**.
3. Build Command: `npm run build`.
4. Output Directory: `dist`.
5. The included [`vercel.json`](file:///C:/Users/PriyaDharshini%20R/OneDrive/Desktop/isha_ui/vercel.json) ensures SPA routing rewrites all routes (`/shop`, `/product/:slug`, `/cart`, etc.) to `/index.html` without 404 errors on browser refresh.

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
