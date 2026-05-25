# CarSim
AutoFinance Simulator — Complete Product & UI/UX Specification

# Project Overview

## Project Name
AutoFinance Simulator

## Project Type
Web-based Car Financing & Vehicle Sales Simulation Platform

## Main Objective
The goal of this project is to build a modern web application for car dealerships and vehicle financing agencies.

The platform allows sales agents to simulate vehicle purchases for customers and instantly calculate:

- Down payment (Apport)
- Loan amount
- Monthly payment (Traite)
- Interest rate calculations
- Financing duration
- Optional services
- Mandatory services
- Discounts and promotions
- Final repayment cost

This project is also designed as a technical learning project to practice:

- C++
- REST APIs
- Web Services
- Frontend Development
- JavaScript
- Financial Calculations
- Software Architecture
- UI/UX Design
- Full-stack Development

---

# Target Users

## 1. Sales Agents
Employees inside dealerships who create financing simulations for customers.

## 2. Customers
People who want to estimate how much they can pay monthly before purchasing a vehicle.

## 3. Admins
Administrators who manage vehicles, pricing, services, and promotions.

---

# Website Goals

The website should feel:

- Professional
- Premium
- Modern automotive style
- Clean and minimal
- Fast and responsive
- Easy to use during real customer meetings

The design inspiration should combine:

- Tesla website
- BMW configurator
- Mercedes financing portals
- Modern SaaS dashboards

---

# UI/UX Design Requirements

# General Style

## Theme
Modern automotive fintech platform.

## Color Palette

### Primary Colors
- Dark blue
- Black
- White
- Metallic gray

### Accent Colors
- Electric blue
- Green for success states
- Orange for warnings

---

# Typography

## Font Style
Modern sans-serif fonts.

Recommended:
- Inter
- Poppins
- Roboto

---

# Layout Style

The UI should use:
- Rounded cards
- Soft shadows
- Smooth transitions
- Glassmorphism effects (optional)
- Responsive grid layouts
- Large modern buttons
- Interactive charts

---

# Website Pages

# 1. Landing Page

## Goal
Present the platform professionally.

## Sections

### Hero Section
Large banner with:
- Luxury car background
- Modern financing dashboard preview
- Main CTA button

Headline example:
"Smart Vehicle Financing Simulation Platform"

Subheadline:
"Create instant car financing simulations for your customers."

Buttons:
- Start Simulation
- View Demo

---

### Features Section

Cards showing:
- Financing calculation
- Vehicle management
- PDF generation
- Customer management
- Analytics dashboard

---

### Statistics Section

Animated counters:
- Simulations generated
- Vehicles managed
- Financing success rate

---

### Testimonials Section

Fake dealership testimonials.

---

### Footer
- Company links
- Social media
- Contact information
- Legal pages

---

# 2. Login Page

## Features
- Email login
- Password login
- Remember me
- Forgot password

## UI Style
Centered glassmorphism card.

Background:
- Dark blurred luxury car image.

---

# 3. Dashboard

# Main Dashboard Layout

## Sidebar Navigation

Sections:
- Dashboard
- New Simulation
- Customers
- Vehicles
- Financing Plans
- Reports
- Analytics
- Settings

---

## Top Navbar

Contains:
- User profile
- Notifications
- Search bar
- Theme switcher

---

## Dashboard Widgets

Cards displaying:
- Total simulations
- Total sales
- Active customers
- Revenue generated

Charts:
- Monthly sales chart
- Financing distribution
- Loan duration statistics

---

# 4. New Financing Simulation Page

This is the MOST IMPORTANT page.

# Page Layout

The page should be split into 2 main sections:

## Left Side
Input form.

## Right Side
Live simulation preview.

---

# Simulation Form Fields

## Customer Information

Fields:
- Full name
- Phone number
- Email
- Monthly salary
- Employment type
- Credit score

---

## Vehicle Information

Fields:
- Vehicle brand
- Vehicle model
- Vehicle year
- Vehicle price

Dropdown examples:
- BMW
- Mercedes
- Audi
- Toyota
- Tesla

---

## Financing Options

Fields:
- Deposit percentage
- Financing duration
- Interest rate
- Insurance option
- Mandatory services
- Optional services
- Discount amount

---

# Live Simulation Result Card

This section updates automatically in real-time.

## Must Display

- Vehicle price
- Assiette
- Deposit amount
- Loan amount
- Monthly payment
- Total interest
- Final repayment amount

---

# Example Financial Logic

## Assiette Formula

```text
assiette =
vehicle_price
+ mandatory_services
+ optional_services
- discount
```

## Deposit Formula

```text
deposit =
assiette × deposit_rate
```

## Loan Formula

```text
loan_amount =
assiette - deposit
```

## Monthly Payment Formula

```text
monthly_payment =
(P × r × (1 + r)^n)
/
((1 + r)^n - 1)
```

Where:
- P = loan amount
- r = monthly interest rate
- n = duration in months

---

# Simulation Actions

Buttons:
- Generate Quote
- Save Simulation
- Export PDF
- Send by Email
- Print

---

# 5. Vehicle Management Page

## Features

- Add vehicle
- Edit vehicle
- Delete vehicle
- Search vehicle
- Filter by:
  - Brand
  - Price
  - Fuel type
  - Availability

---

## Vehicle Cards

Each card should show:
- Vehicle image
- Vehicle name
- Price
- Financing availability
- Quick simulate button

---

# 6. Customer Management Page

## Features

- Customer list
- Search customer
- Customer financing history
- Saved simulations
- Contact information

---

# 7. Reports & Analytics Page

## Charts

- Sales performance
- Most financed vehicles
- Monthly revenue
- Financing durations
- Interest revenue

---

## Graph Types

Use:
- Line charts
- Pie charts
- Bar charts
- KPI cards

---

# Responsive Design Requirements

The website MUST work on:
- Desktop
- Tablet
- Mobile

---

# Mobile UI

On mobile:
- Sidebar becomes collapsible
- Cards become stacked
- Charts become scrollable
- Buttons become full-width

---

# Backend Architecture

# Backend Technology

## Primary Language
C++

## API Type
REST API

---

# Suggested C++ Frameworks

Choose one:
- Crow
- Drogon
- Pistache
- Boost.Beast

---

# Backend Responsibilities

The backend should:
- Receive JSON requests
- Validate data
- Execute financial calculations
- Return JSON responses
- Store simulations
- Manage customers

---

# Example API Request

```json
{
  "vehicle_price": 30000,
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
  "assiette": 31000,
  "deposit_amount": 6200,
  "loan_amount": 24800,
  "monthly_payment": 473.25,
  "total_interest": 3595,
  "total_paid": 34595
}
```

---

# Frontend Technology Suggestions

## Option 1
- HTML
- CSS
- JavaScript

## Option 2 (Recommended)
- React
- Tailwind CSS
- TypeScript

---

# Suggested Frontend Libraries

## UI
- Tailwind CSS
- ShadCN UI

## Charts
- Recharts
- Chart.js

## Icons
- Lucide Icons

## Animations
- Framer Motion

---

# Database Suggestions

Recommended:
- PostgreSQL

Alternative:
- MySQL
- MongoDB

---

# Authentication Features

## Roles

### Admin
Can manage:
- Vehicles
- Pricing
- Financing plans
- Users

### Sales Agent
Can:
- Create simulations
- Save customers
- Generate quotes

---

# Future AI Features

## AI Recommendation System

Suggest:
- Best financing plans
- Vehicles based on salary
- Budget recommendations

---

# PDF Generation

Generate:
- Financing quotation
- Contract preview
- Customer report

---

# Advanced Future Features

## Vehicle Configurator
Choose:
- Color
- Interior
- Wheels
- Packages

---

## Multi-language Support
Languages:
- English
- French
- Arabic

---

# Suggested Folder Structure

```text
frontend/
backend/
database/
docs/
api/
```

---

# Suggested Backend Structure

```text
backend/
├── controllers/
├── services/
├── models/
├── routes/
├── utils/
├── calculations/
└── main.cpp
```

---

# Suggested Frontend Structure

```text
frontend/
├── components/
├── pages/
├── layouts/
├── services/
├── hooks/
├── assets/
└── app/
```

---

# Desired UX Feeling

The application should feel:
- Professional
- Smooth
- Modern
- Premium
- Fast
- Similar to a real dealership financing system

The user experience should prioritize:
- Speed
- Simplicity
- Clarity
- Real-time feedback

---

# Final Goal

The final platform should look like a real commercial SaaS product used by:
- Car dealerships
- Financing companies
- Vehicle agencies

while also serving as a strong technical portfolio project demonstrating:
- Backend engineering
- C++ expertise
- API development
- Financial logic
- Full-stack web development
- Modern UI/UX design
