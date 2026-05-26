
# AutoFinance Simulator — Enterprise Design System & Implementation Blueprint

> Based directly on the official UI/UX specification PDF prototype.

---

# Project Identity

## Product Name
AutoFinance Simulator

## Version
2.0

## Theme
Modern Automotive Fintech — Dark Mode

## Official Stack

- React
- TypeScript
- Tailwind CSS
- Lucide Icons
- Inter Font
- Poppins Font
- Framer Motion
- Recharts

The UI must preserve the EXACT same:
- Colors
- Typography
- Glassmorphism
- Layout system
- Animations
- Spacing
- Component hierarchy
- Automotive premium feeling

Source specification extracted from uploaded prototype PDF. fileciteturn2file0L1-L20

---

# Official Color System

## Primary Scale

| Token | Hex |
|---|---|
| Primary 950 | #172554 |
| Primary 900 | #1e3a8a |
| Primary 800 | #1e40af |
| Primary 700 | #1d4ed8 |
| Primary 600 | #2563eb |
| Primary 500 | #3b82f6 |
| Primary 400 | #60a5fa |
| Primary 300 | #93c5fd |

---

## Dark Theme

| Token | Hex |
|---|---|
| Dark 900 | #0a0a0f |
| Dark 800 | #12121a |
| Dark 700 | #1a1a2e |
| Dark 600 | #22223a |
| Dark 500 | #2a2a42 |

---

## Accent Colors

| Token | Hex |
|---|---|
| Electric Blue | #00d4ff |
| Success | #10b981 |
| Warning | #f59e0b |
| Danger | #ef4444 |

---

# Official Typography

## Fonts

### Main Font
Inter

### Display Font
Poppins

---

## Typography Scale

| Role | Size |
|---|---|
| Hero Title | 72px |
| H1 | 48px |
| H2 | 36px |
| H3 | 24px |
| H4 | 18px |
| Body | 16px |
| Body Small | 14px |
| Caption | 12px |

---

# Official Design Language

## UI Style

The application uses:

- Dark premium dashboard
- Automotive fintech style
- Glassmorphism
- Soft blur surfaces
- Electric blue highlights
- Rounded cards
- Floating shadows
- Real-time calculation previews

---

# Glassmorphism System

## Main Glass Class

```css
.glass {
  background: rgba(255,255,255,0.05);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(255,255,255,0.1);
}
```

---

## Dark Glass

```css
.glass-dark {
  background: rgba(10,10,15,0.7);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(255,255,255,0.05);
}
```

---

# Gradient System

## Gradient Text

```css
.gradient-text {
  background: linear-gradient(
    135deg,
    #3b82f6 0%,
    #00d4ff 100%
  );

  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
```

---

# Hero Background

```css
.hero-bg {
  background: linear-gradient(
    135deg,
    #0a0a0f 0%,
    #1a1a2e 50%,
    #172554 100%
  );
}
```

---

# Layout System

## Responsive Grid

| Breakpoint | Layout |
|---|---|
| Mobile | 1 column |
| Tablet | 2 columns |
| Desktop | 3–4 columns |
| Wide | 4–6 columns |

---

# Navbar Specification

## Navbar Features

- Fixed top navigation
- Glass blur background
- Gradient logo
- Navigation links
- Notification bell
- User profile avatar

## Navbar Height

64px

---

# Sidebar Specification

## Width

256px

## Active Item Style

- Blue transparent background
- Left blue border
- White text

---

# Hero Section

## Left Side

Contains:
- Main marketing title
- Subtitle
- CTA buttons

## Right Side

Live financing preview card.

---

# Hero Effects

Use:
- Large blurred gradient circles
- Blue glow lighting
- Floating premium elements

---

# Buttons System

# Primary Button

```css
background: linear-gradient(
135deg,
#2563eb,
#3b82f6
);
```

Features:
- Glow shadow
- Rounded corners
- Scale hover effect
- White bold text

---

# Secondary Button

Glass transparent button.

---

# Ghost Button

Transparent minimal hover button.

---

# Cards System

# Standard Card

Features:
- Glass background
- Rounded 24px
- Hover lift animation
- Premium shadows

---

# Highlighted Card

Features:
- Blue highlighted border
- Premium hover effect
- Glass background

---

# Dark Surface Card

Features:
- Deep gradient background
- Used for:
  - Analytics
  - Live preview
  - Financial calculations

---

# Vehicle Card Design

## Structure

- Image area
- Gradient overlay
- Availability badge
- Car icon
- Price
- Tags
- Quick simulate button

---

# Form Design

# Inputs

## Input Style

- Dark background
- Rounded corners
- Soft border
- White text
- Blue glow on focus

---

# Input with Icon

- Left aligned icon
- 20px icon size
- 40px left padding

---

# Dropdown Style

- Same style as text input
- Custom arrow
- Dark theme

---

# Tables System

## Table Style

- Glass container
- Rounded corners
- Hover rows
- Uppercase headers
- Soft dividers

---

# Charts System

## Supported Charts

- Bar charts
- Progress bars
- Donut charts

---

# Chart Colors

Use:
- Blue gradients
- Electric blue highlights
- Success green
- Warning orange

---

# Simulation Page

# PRIMARY PAGE

The simulation page is the core business page.

---

# Layout

## Left Side

Financing form.

## Right Side

Sticky live preview card.

---

# Customer Information Fields

- Full Name
- Phone Number
- Email
- Monthly Salary

---

# Vehicle Information Fields

- Brand
- Model
- Year
- Price

---

# Financing Fields

- Deposit rate
- Duration
- Interest rate
- Discount
- Mandatory services
- Optional services

---

# Live Preview Card

## Must Display

- Vehicle price
- Assiette
- Deposit
- Loan amount
- Monthly payment
- Total interest
- Total repayment

---

# Monthly Payment Style

Use:
- Large typography
- Gradient text
- Premium glow
- Highlight background

---

# Financial Formulas

## Assiette Formula

```text
assiette =
vehicle_price
+ mandatory_services
+ optional_services
- discount
```

---

## Deposit Formula

```text
deposit =
assiette × deposit_rate
```

---

## Loan Formula

```text
loan =
assiette - deposit
```

---

## Monthly Payment Formula

```text
monthly_payment =
(P × r × (1 + r)^n)
/
((1 + r)^n - 1)
```

---

# Dashboard Widgets

## KPI Cards

Display:
- Simulations
- Revenue
- Customers
- Conversion rate

---

# Widget Style

- Glass cards
- Hover animations
- Icons
- Trend indicators

---

# Analytics

## Components

- Revenue chart
- Financing distribution
- Vehicle distribution
- Donut charts

---

# Status Pills

## Success

Green transparent background.

## Warning

Orange transparent background.

## Danger

Red transparent background.

## Info

Blue transparent background.

---

# Icons

## Official Icon Library

Lucide Icons

---

# Common Icons

| Feature | Icon |
|---|---|
| Dashboard | layout-dashboard |
| Vehicles | car |
| Customers | users |
| Financing | calculator |
| Reports | file-text |
| Notifications | bell |
| User | user |
| Search | search |
| Save | save |
| PDF | download |
| Email | mail |
| Print | printer |

---

# Animations

# Card Hover

```css
transform: translateY(-4px);
```

---

# Button Hover

```css
transform: scale(1.02);
```

---

# Main Transition

```css
transition:
all 0.3s cubic-bezier(
0.4,
0,
0.2,
1
);
```

---

# Loading States

## Button Loading

- Spinner icon
- Disabled opacity
- Loading text

---

# Toast Notifications

## Success Toast

- Green left border
- Check-circle icon

## Error Toast

- Red left border
- Alert icon

---

# Mobile Responsive Rules

## Mobile

- Sidebar hidden
- Hamburger menu
- Full-width buttons
- Single column layout

---

# Tablet

- 2-column forms
- Collapsible sidebar

---

# Desktop

- Full sidebar
- Sticky live preview
- Multi-column dashboard

---

# Official Tailwind Extension

```js
fontFamily: {
  sans: ['Inter', 'system-ui', 'sans-serif'],
  display: ['Poppins', 'system-ui', 'sans-serif'],
}
```

---

# Official Tailwind Colors

```js
colors: {
  primary: {
    500: '#3b82f6',
    700: '#1d4ed8',
    950: '#172554',
  },

  dark: {
    900: '#0a0a0f',
    800: '#12121a',
    700: '#1a1a2e',
  },

  accent: {
    electric: '#00d4ff',
    success: '#10b981',
    warning: '#f59e0b',
    danger: '#ef4444',
  }
}
```

---

# Recommended Frontend Stack

- React
- TypeScript
- Tailwind CSS
- Framer Motion
- Recharts
- ShadCN UI
- Lucide React

---

# Backend Architecture

## Backend Language

C++

## API Style

REST API

## Suggested Frameworks

- Drogon
- Crow
- Pistache

---

# Backend Responsibilities

- Receive JSON
- Execute calculations
- Return financing results
- Store simulations
- Manage vehicles
- Manage customers

---

# Example API Request

```json
{
  "vehicle_price": 45000,
  "mandatory_services": 1200,
  "optional_services": 800,
  "discount": 1000,
  "deposit_rate": 20,
  "duration_months": 60,
  "interest_rate": 5.5
}
```

---

# Example API Response

```json
{
  "assiette": 46000,
  "deposit_amount": 9200,
  "loan_amount": 36800,
  "monthly_payment": 701.23,
  "total_interest": 5274,
  "total_repayment": 42074
}
```

---

# Suggested Frontend Structure

```text
frontend/
├── app/
├── components/
├── pages/
├── layouts/
├── hooks/
├── services/
├── assets/
├── styles/
└── utils/
```

---

# Suggested Backend Structure

```text
backend/
├── controllers/
├── routes/
├── services/
├── calculations/
├── models/
├── utils/
└── main.cpp
```

---

# Accessibility Rules

- Focus-visible support
- Minimum contrast ratios
- Keyboard navigation
- Accessible labels
- ARIA live regions

---

# Final Product Goal

The final application should feel like a REAL commercial automotive financing SaaS platform used by:

- Car dealerships
- Vehicle financing companies
- Automotive agencies

while showcasing:
- Modern UI/UX
- Full-stack engineering
- Professional frontend architecture
- C++ backend integration
- Real-time financial calculations
