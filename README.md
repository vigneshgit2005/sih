# Connect & Cope - Student Mental Health Platform

[![Next.js](https://img.shields.io/badge/Next.js-15.3.3-black.svg?style=flat&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.7.3-blue.svg?style=flat&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3.4.1-blue.svg?style=flat&logo=tailwind-css)](https://tailwindcss.com/)
[![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-Elegant%20UI-blue.svg?style=flat&logo=shadcn)](https://ui.shadcn.com/)
[![Genkit AI](https://img.shields.io/badge/Genkit%20AI-Firebase%20AI-orange.svg?style=flat&logo=firebase)](https://firebase.google.com/docs/genkit)

A comprehensive, stigma-free mental health support platform designed specifically for university students. Provides 24/7 AI-powered chatbot support, professional counseling booking, curated resources, and anonymous peer forums.

## 🚀 Features

### 🎯 **AI Chatbot Support**
- **24/7 Availability**: Immediate, private conversations with AI trained for student mental health
- **Anxiety Management**: Specialized flows for anxiety coping strategies
- **Personalized Coping Tips**: Tailored recommendations based on user input
- **Resource Recommendations**: AI suggests relevant articles/videos/guides

### 📅 **Professional Counseling**
- Easy session booking with university counselors
- Confidential appointment scheduling
- Calendar integration with `react-day-picker`

### 📚 **Resource Hub**
- Curated library of mental wellness content
- Articles, videos, audio guides
- Organized by topic for easy discovery

### 👥 **Peer Support Forum**
- Safe, anonymous, moderated community space
- Connect with fellow students
- Share experiences and support each other

### ✨ **Modern UI/UX**
- Responsive design (mobile-first)
- Dark mode support
- shadcn/ui components
- Smooth animations and transitions
- Accessibility-first (ARIA compliant)

## 🛠 Tech Stack

```
Frontend: Next.js 15.3.3 (App Router) + TypeScript 5.7.3
Styling: Tailwind CSS 3.4.1 + shadcn/ui
AI: Firebase Genkit + Google AI (Gemini)
Charts: Recharts
Forms: React Hook Form + Zod
State: React Context
UI Libs: @radix-ui/react, lucide-react icons
Deployment: Vercel / Firebase App Hosting
```

## 📱 Live Demo
```
Local: http://localhost:9002
Network: http://192.168.1.15:9002 (when running)
```

## 🏗 Project Structure

```
src/
├── app/                 # Next.js App Router
│   ├── chatbot/         # AI Chatbot interface
│   ├── booking/         # Counseling booking
│   ├── resources/       # Resource library
│   ├── forum/           # Peer support
│   └── admin/           # Admin dashboard
├── components/          # Reusable components
│   ├── ui/             # shadcn/ui components
│   └── chatbot/        # Chatbot specific
├── ai/                 # Genkit AI flows
│   ├── flows/          # Specialized AI flows
│   └── genkit.ts       # AI configuration
└── lib/                # Utilities & data
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ (recommended: 24.x)
- npm 10+

### Installation
```bash
npm install
```

### Development Server
```bash
npm run dev
# Server starts at http://localhost:9002
```

### Build & Start
```bash
npm run build
npm start
```

### Available Scripts
```bash
npm run dev      # Development server with Turbopack
npm run genkit:dev  # Genkit AI dev server
npm run build    # Production build
npm run start    # Production server
npm run lint     # ESLint
npm run typecheck # TypeScript check
```

## 🌐 AI Features (Genkit)

Three specialized AI flows:
1. **ai-chatbot-anxiety-management.ts** - Anxiety coping strategies
2. **ai-chatbot-personalized-coping-tips.ts** - Personalized recommendations
3. **ai-chatbot-resource-recommendation.ts** - Resource suggestions

Configure your Firebase/Google AI API keys in environment variables.

## 📊 Key Pages & Components

| Route | Description | Key Components |
|-------|-------------|----------------|
| `/` | Homepage | Hero, Feature Cards |
| `/chatbot` | AI Chat Interface | `ChatInterface.tsx` |
| `/booking` | Session Booking | `BookingForm.tsx` |
| `/resources` | Resource Library | `ResourceList.tsx` |
| `/forum` | Peer Forum | `Forum.tsx` |
| `/admin` | Admin Dashboard | `Dashboard.tsx` |

## 🎨 UI Components (shadcn/ui)

- **Data Display**: Card, Table, Badge, Progress
- **Forms**: Form, Input, Select, Checkbox, RadioGroup
- **Navigation**: Menubar, Tabs, Accordion
- **Modals**: Dialog, AlertDialog, Sheet
- **Layout**: Sidebar, Carousel, ScrollArea

## 🔧 Customization

### Tailwind Config
Edit `tailwind.config.ts` for custom colors/spacing.

### Theme
Update `globals.css` for custom CSS variables.

### Components
Add new shadcn/ui components:
```bash
npx shadcn-ui@latest add [component]
```

## 🚀 Deployment

### Vercel (Recommended)
```bash
npm i -g vercel
vercel --prod
```

### Firebase App Hosting
Configure `apphosting.yaml` and deploy via Firebase CLI.

### Docker
```dockerfile
# Dockerfile
FROM node:20-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY . .
RUN npm run build
EXPOSE 9002
CMD ["npm", "start"]
```

## 📈 Performance

- **Turbopack**: Lightning-fast dev server
- **App Router**: Next.js 15+ optimized routing
- **Server Components**: Reduced bundle size
- **Image Optimization**: Next.js Image component
- **Code Splitting**: Automatic by Next.js

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/)
- [shadcn/ui](https://ui.shadcn.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Firebase Genkit](https://firebase.google.com/docs/genkit)
- [Radix UI](https://www.radix-ui.com/)

---

⭐ **Star this repo if you found it helpful!** ⭐
