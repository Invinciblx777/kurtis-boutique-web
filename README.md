# Kurtis Boutique Web

An elegant, high-performance e-commerce platform built for **Kurtis Boutique**. The application features a modern storefront, a fully integrated checkout pipeline, a custom admin dashboard, and progressive web app (PWA) capabilities.

## 🚀 Features

### Customer Experience
- **Modern Storefront:** Server-side rendered (ISR) product pages and shop-by-look reels.
- **Rich Product Galleries:** Swipeable image galleries for touch devices and "quick view" modals.
- **Customisation & Add-ons:** Dedicated customisation query forms and dynamic add-on charges.
- **Seamless Checkout:** Razorpay integration for secure payments with fallback handling and recovery.
- **Order Tracking:** Integrated tracking timeline and automated email/WhatsApp notifications.
- **PWA Ready:** Installable on mobile devices with offline support and push notifications.
- **Optimized Performance:** Blazing fast image loading via `next/image` and CDN caching.

### Admin & Management
- **Dashboard:** Instant-render admin panel to manage products, categories, and inventory.
- **Order Management:** View, update, and manage incoming orders, track shipments, and delete unneeded entries.
- **Image Uploads:** Drag-to-reorder interface for product image management.
- **Notifications:** Receive instant WhatsApp and Email alerts for new orders.
- **Role-Based Access:** Secure Supabase RLS policies and server-side session validations for admin accounts.

## 🛠 Tech Stack

- **Framework:** [Next.js](https://nextjs.org/) (App Router, ISR, Server Actions)
- **Styling:** [Tailwind CSS](https://tailwindcss.com/) & [Framer Motion](https://www.framer.com/motion/)
- **UI Components:** [shadcn/ui](https://ui.shadcn.com/), Radix UI, Lucide React
- **State & Forms:** [Zustand](https://zustand-demo.pmnd.rs/), React Hook Form, Zod
- **Backend & Database:** [Supabase](https://supabase.com/) (Auth, PostgreSQL, Storage)
- **Payments:** [Razorpay](https://razorpay.com/)
- **SEO & Performance:** `next-sitemap`, dynamic meta tags, and structured schema markup

## ⚙️ Getting Started

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) (v18+) and your preferred package manager (npm, yarn, pnpm) installed. You will also need a Supabase project and a Razorpay account.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Invinciblx777/kurtis-boutique-web.git
   cd kurtis-boutique-web
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure Environment Variables:**
   Create a `.env.local` file in the root directory and add the following keys:
   ```env
   # Supabase Configuration
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_project_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key

   # Razorpay Configuration
   NEXT_PUBLIC_RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret

   # App Configuration
   NEXT_PUBLIC_SITE_URL=http://localhost:3000
   ```

4. **Run the development server:**
   ```bash
   npm run dev
   # or
   yarn dev
   ```
   Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📁 Project Structure

- `app/` - Next.js App Router pages, layouts, and API routes.
- `components/` - Reusable UI elements, shadcn components, and forms.
- `lib/` - Utility functions, validation schemas (Zod), and Supabase client initializers.
- `public/` - Static assets, images, and PWA manifests.

## 📄 License

This project is proprietary and confidential. Unauthorized copying of this file, via any medium is strictly prohibited.
