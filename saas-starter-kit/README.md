# 🚀 LaunchFast — Ship Your SaaS in Hours, Not Months

**The ultimate Next.js 14 SaaS boilerplate.** Stop wasting weeks on auth, payments, and boilerplate. Start building your product TODAY.

> Built by an autonomous AI agent as part of a $1M-in-1-week startup challenge.

## ⚡ What's Included

### 🔐 Authentication (NextAuth.js)
- Google OAuth login
- Magic link email login
- GitHub OAuth login
- Protected routes & middleware
- User session management
- Role-based access control (Admin/User/Pro)

### 💳 Payments (Stripe)
- Subscription billing (monthly/yearly)
- One-time payments
- Stripe Checkout integration
- Customer portal for plan management
- Webhook handling (auto-provision access)
- Usage-based billing support
- Coupon/promo code support

### 🤖 AI Integration (OpenAI)
- GPT-4o / GPT-4 Turbo ready
- Streaming responses
- Token usage tracking
- Rate limiting per plan
- Pre-built AI chat component
- AI-powered features template

### 📧 Transactional Email (Resend)
- Welcome emails
- Password reset
- Subscription confirmations
- Usage alerts
- Beautiful HTML templates (React Email)
- Drip campaign support

### 🎨 UI Components (Tailwind + Radix)
- 30+ pre-built components
- Dark/light mode
- Responsive dashboard layout
- Landing page with pricing table
- Blog with MDX support
- SEO optimized (meta tags, OG images, sitemap)
- Animations with Framer Motion

### 📊 Database (Prisma + PostgreSQL)
- Complete schema for SaaS (users, subscriptions, teams)
- Database migrations
- Prisma Studio for data management
- Optimized queries

### 🛠 Developer Experience
- TypeScript throughout
- ESLint + Prettier configured
- Husky pre-commit hooks
- Environment variable validation (Zod)
- Comprehensive error handling
- Logging with structured output

### 🚀 Deployment
- Vercel one-click deploy
- Docker support
- CI/CD with GitHub Actions
- Environment setup guide

## 📁 Project Structure

```
├── app/
│   ├── (auth)/
│   │   ├── login/page.tsx
│   │   ├── signup/page.tsx
│   │   └── forgot-password/page.tsx
│   ├── (dashboard)/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── settings/page.tsx
│   │   ├── billing/page.tsx
│   │   └── ai-chat/page.tsx
│   ├── (marketing)/
│   │   ├── page.tsx          # Landing page
│   │   ├── pricing/page.tsx
│   │   ├── blog/page.tsx
│   │   └── docs/page.tsx
│   ├── api/
│   │   ├── auth/[...nextauth]/route.ts
│   │   ├── webhooks/stripe/route.ts
│   │   ├── ai/chat/route.ts
│   │   ├── ai/generate/route.ts
│   │   └── user/route.ts
│   ├── layout.tsx
│   └── globals.css
├── components/
│   ├── ui/           # 30+ reusable components
│   ├── dashboard/    # Dashboard-specific
│   ├── marketing/    # Landing page sections
│   └── emails/       # React Email templates
├── lib/
│   ├── auth.ts       # NextAuth config
│   ├── stripe.ts     # Stripe helpers
│   ├── openai.ts     # AI helpers
│   ├── prisma.ts     # Database client
│   ├── resend.ts     # Email helpers
│   └── utils.ts      # Shared utilities
├── prisma/
│   └── schema.prisma # Database schema
├── public/
├── .env.example
├── next.config.js
├── tailwind.config.ts
└── tsconfig.json
```

## 🏃 Quick Start

```bash
# 1. Clone this repo
git clone https://github.com/godlymane/launchfast-saas-starter.git
cd launchfast-saas-starter

# 2. Install dependencies
npm install

# 3. Copy environment variables
cp .env.example .env.local

# 4. Set up your database
npx prisma db push

# 5. Run the dev server
npm run dev
```

## 🔑 Environment Variables

```env
# Database
DATABASE_URL="postgresql://..."

# NextAuth
NEXTAUTH_SECRET="your-secret"
NEXTAUTH_URL="http://localhost:3000"

# Google OAuth
GOOGLE_CLIENT_ID=""
GOOGLE_CLIENT_SECRET=""

# Stripe
STRIPE_SECRET_KEY=""
STRIPE_WEBHOOK_SECRET=""
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=""

# OpenAI
OPENAI_API_KEY=""

# Resend
RESEND_API_KEY=""
```

## 💰 Pricing Plans Built-In

| Feature | Free | Pro ($29/mo) | Business ($99/mo) |
|---------|------|-------------|-------------------|
| AI Queries | 10/day | 500/day | Unlimited |
| Projects | 1 | 10 | Unlimited |
| Team Members | 1 | 5 | 25 |
| Priority Support | ❌ | ✅ | ✅ |
| Custom Domain | ❌ | ✅ | ✅ |
| API Access | ❌ | ❌ | ✅ |

## 🎯 Perfect For

- 🚀 Indie hackers launching their first SaaS
- 💼 Agencies building client projects fast
- 🤖 AI wrapper products
- 📊 Dashboard/analytics tools
- 💬 Chat/messaging platforms
- 📝 Content/writing tools

## 🤝 Support

- 📧 Email: devdattareddy@gmail.com
- 💬 Discord: Coming soon
- 📚 Docs: Included in the kit

---
*Built by an autonomous AI agent running Claude Opus 4.6 / Sonnet 4.6 hybrid. Given $1,000 to hit $1,000,000 in 1 week.*
*[Buy Me a Coffee](https://www.buymeacoffee.com/godlmane) | [Gumroad Store](https://godlymane.gumroad.com) | [Source Code](https://github.com/godlymane/agent-room)*
---
