# ⚡ Winds AI Pro v2.0

[![Next.js 15](https://img.shields.io/badge/Next.js-15.0_App_Router-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma)](https://prisma.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o_Mini_Intelligence-412991?style=for-the-badge&logo=openai)](https://openai.com)
[![Stripe](https://img.shields.io/badge/Stripe-Checkout_&_Webhooks-635BFF?style=for-the-badge&logo=stripe)](https://stripe.com)
[![Bilingual i18n](https://img.shields.io/badge/i18n-English_%26_Português-10B981?style=for-the-badge)](https://kiptecnologia.github.io/winds-pro/)
[![By Kip Tecnologia](https://img.shields.io/badge/By-Kip_Tecnologia-059669?style=for-the-badge)](https://github.com/KipTecnologia)
[![Live Demo](https://img.shields.io/badge/Live-Demo_Ready-emerald?style=for-the-badge&logo=googlechrome)](https://kiptecnologia.github.io/winds-pro/)

> **English**: Turnkey **AI Audio & Knowledge Feed Intelligence Studio & Micro-SaaS Boilerplate**. Built with **Next.js 15 App Router**, **TypeScript**, **Prisma ORM**, **Universal RSS & Podcast XML Parser**, **OpenAI Executive Summarization Engine**, and **Stripe Subscriptions**.  
> **Português**: Estúdio completo de **Inteligência de Feeds RSS e Player de Podcasts com IA**. Construído com **Next.js 15**, **Prisma ORM**, **Parser Universal de RSS/Podcasts**, **Resumos Executivos OpenAI** e **Stripe**. Engineered by **[Kip Tecnologia](https://github.com/KipTecnologia)**.

---

## ⚡ Live Interactive Demo (Bilingual EN / PT)

Experience the live podcast player, RSS reader, and instant AI summarizer with instant English 🇺🇸 / Portuguese 🇧🇷 switcher:  
👉 **[https://kiptecnologia.github.io/winds-pro/](https://kiptecnologia.github.io/winds-pro/)**

- **🎙️ Audio Podcast Player**: Persistent audio scrubber with waveform frequency pulses and variable playback speeds (1x to 2.5x).
- **📡 Universal RSS Parser**: Instant ingestion of news feeds, newsletters, and podcasts.
- **✨ AI Executive Briefings**: Condenses lengthy essays and episodes into 3 key actionable takeaways.
- **💳 Stripe Monetization Showcase**: Live checkout demonstration for recurrent subscriptions ($19/mo) and lifetime access ($89).

---

## 🏗️ Production Micro-SaaS Architecture

```
winds-pro/
├── prisma/
│   └── schema.prisma                # User, FeedSource, UserFeed, FeedArticle & Bookmark
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── feeds/
│   │   │   │   ├── parse/route.ts       # Universal RSS & Podcast XML parser
│   │   │   │   └── summarize/route.ts   # OpenAI executive brief & takeaways generator
│   │   │   └── stripe/
│   │   │       ├── checkout/route.ts    # Stripe Checkout session creator
│   │   │       └── webhook/route.ts     # Automated plan upgrade webhook
│   │   ├── globals.css                  # Custom waveform animations & audio styles
│   │   ├── layout.tsx                   # SEO & Root Layout
│   │   └── page.tsx                     # Full-featured audio player & reader dashboard
│   ├── lib/
│   │   ├── db.ts                        # Prisma client singleton
│   │   ├── feeds/
│   │   │   └── parser.ts                # Native XML parser with audio enclosure extraction
│   │   ├── ai/
│   │   │   └── summarizer.ts            # OpenAI prompt engineering with offline fallback
│   │   └── stripe.ts                    # Stripe plans & billing config
│   └── types/
│       └── feed.ts                      # TypeScript types for feeds, articles & audio
├── .env.example                         # Documented environment variables
├── package.json
└── README.md
```

---

## 💰 Built-in Monetization & Business Model

Winds AI Pro comes with a pre-configured recurring software business model:

| Plan | Price (Global) | Price (Brazil) | Features |
| :--- | :---: | :---: | :--- |
| **Curious Reader** | $0 | R$ 0 | Up to 5 feeds, native audio player, 3 AI summaries/day |
| **Pro Curator Monthly** | $19 / mo | R$ 89 / mês | Up to 50 feeds, unlimited AI summaries, 2.5x audio speed, 1-click Notion export |
| **Lifetime Studio** | $89 once | R$ 399 único | Unlimited feeds, full TypeScript source code, zero royalties, VIP support |

---

## 🚀 Quick Start Guide (English)

### 1. Clone & Install
```bash
git clone https://github.com/KipTecnologia/winds-pro.git
cd winds-pro
npm install
```

### 2. Configure Environment Variables
```bash
cp .env.example .env
```
Fill in:
- `DATABASE_URL`: Defaults to local SQLite (`file:./dev.db`) for instant local run.
- `OPENAI_API_KEY`: For live AI summaries and transcript insights.
- `STRIPE_SECRET_KEY`: For monetization checkout.

### 3. Initialize Database & Run
```bash
npx prisma db push
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) to view the application.

---

## 🇧🇷 Guia de Início Rápido (Português)

### 1. Instalação e Execução
```bash
git clone https://github.com/KipTecnologia/winds-pro.git
cd winds-pro
npm install
cp .env.example .env
npx prisma db push
npm run dev
```

### 2. Adicionar Feeds RSS e Podcasts
A aplicação suporta qualquer link de RSS de notícias ou podcast em XML (Substack, Medium, TechCrunch, Apple Podcasts).

---

## 🏢 About Kip Tecnologia

**Winds AI Pro** is engineered and maintained by **Kip Tecnologia**.

- **Website**: [kiptecnologia.com.br](https://kiptecnologia.com.br)
- **GitHub**: [github.com/KipTecnologia](https://github.com/KipTecnologia)
- **Support**: `contato@kiptecnologia.com.br`

---

## 💎 Commercial Licensing vs. Public Demo

| Feature / Asset | Public Interactive Demo (Free) | Commercial License & Full Boilerplate (Paid) |
| :--- | :---: | :---: |
| **Interactive Feed Reader & Audio Player** | ✅ Free Access | ✅ Included |
| **Bilingual Switcher (EN / PT)** | ✅ Included | ✅ Included |
| **Distraction-Free Focus Reader** | ✅ Included | ✅ Included |
| **Next.js 15 App Router Full Source** | ❌ (Commercial) | ✅ **100% Unlocked** |
| **Prisma ORM & SQLite/PostgreSQL Database** | ❌ (Commercial) | ✅ **Production Models** |
| **Universal RSS, Atom & Podcast XML Parser** | ❌ (Commercial) | ✅ **Production Endpoints** |
| **OpenAI GPT-4o Mini Summarization Engine** | ❌ (Commercial) | ✅ **Turnkey AI Pipeline** |
| **Stripe Checkout & Automated Webhooks** | ❌ (Commercial) | ✅ **Turnkey Setup** |
| **100% White-Label Rights (Launch your own SaaS)** | ❌ (Evaluation only) | ✅ **Full Commercial Rights** |
| **Lifetime Updates & Discord VIP Access** | ❌ (Evaluation only) | ✅ **Included** |

👉 **[Acquire Commercial License & Full Boilerplate on Gumroad](https://rancharia.gumroad.com)**

---

## 📄 License

This repository is governed by the **Kip Tecnologia Commercial & Evaluation License (v2.0)**. The interactive demo and public assets are available for evaluation purposes. Commercial reproduction, distribution, and SaaS operation require a valid Commercial License from Kip Tecnologia. Copyright (c) 2026 Kip Tecnologia.
