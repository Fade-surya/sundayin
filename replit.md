# Sunday - E-commerce Website

## Overview
Sunday is an e-commerce reselling website with a customer-facing storefront and admin dashboard. Built with Next.js and PostgreSQL.

## Project Structure
```
sunday-store/
├── app/
│   ├── api/               # API routes
│   │   ├── auth/          # Authentication endpoints
│   │   ├── products/      # Product CRUD
│   │   ├── admins/        # Admin management
│   │   ├── categories/    # Category endpoints
│   │   └── init/          # Database initialization
│   ├── admin/             # Admin pages
│   │   ├── login/         # Admin login page
│   │   └── dashboard/     # Admin dashboard
│   ├── product/[id]/      # Product detail page
│   └── page.tsx           # Homepage/storefront
├── components/            # React components
│   ├── Header.tsx
│   ├── Footer.tsx
│   └── ProductCard.tsx
└── lib/                   # Utilities
    ├── db.ts              # Database connection
    └── auth.ts            # Authentication logic
```

## Features
- Customer storefront with product listings (Amazon-style grid)
- Product search and category filtering
- Admin dashboard for product management
- Multi-admin support (Super Admin can add other admins)
- Instagram link integration for products
- Original price vs sale price with discount display

## Admin Access
- **Super Admin Email**: assooryamsu80@gmail.com
- **Password**: sreevava123
- Super admin can add/remove other admins
- All admins can manage products

## Tech Stack
- Next.js 16 with TypeScript
- PostgreSQL database
- Tailwind CSS
- bcryptjs for password hashing
- JWT for authentication

## Deployment
Configured for Vercel deployment. The app binds to port 5000 in development.

## Database Tables
- `admins` - Admin users with email/password auth
- `products` - Product catalog with prices, images, stock
- `categories` - Product categories

## Recent Changes
- December 2024: Initial build with full e-commerce functionality
