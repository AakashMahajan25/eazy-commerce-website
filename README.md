# 🛒 Eazy Commerce Website

A modern, high-performance e-commerce website built with Next.js 15, React 19, TypeScript, and Tailwind CSS. This project provides a solid foundation for building scalable e-commerce applications with the latest web technologies.

## ✨ Features

- **⚡ Performance First**: Built with Next.js 15 and Turbopack for lightning-fast development
- **🔷 Type Safety**: Full TypeScript integration with strict mode enabled
- **🎨 Modern Styling**: Tailwind CSS v4 with built-in dark mode support
- **📱 Responsive Design**: Mobile-first approach with responsive components
- **🚀 App Router**: Leveraging Next.js App Router for optimal performance
- **🔤 Optimized Fonts**: Geist Sans & Geist Mono fonts with automatic optimization
- **♿ Accessibility Ready**: Built with accessibility best practices in mind

## 🛠 Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **Next.js** | 15.3.0 | React framework with App Router |
| **React** | 19.0.0 | UI library with latest features |
| **TypeScript** | 5.x | Type-safe JavaScript development |
| **Tailwind CSS** | 4.x | Utility-first CSS framework |
| **PostCSS** | Latest | CSS processing and optimization |
| **Turbopack** | Built-in | Ultra-fast bundler for development |

## 📋 Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Node.js**: Version 18.17 or higher
- **npm**: Version 9.0 or higher (comes with Node.js)
- **Git**: For version control

### Check your installation:
```bash
node --version  # Should be 18.17+
npm --version   # Should be 9.0+
git --version   # Any recent version
```

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone <repository-url>
cd eazy-commerce-website
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Start Development Server
```bash
npm run dev
```

### 4. Open in Browser
Navigate to [http://localhost:3000](http://localhost:3000) to see your application running.

## 📁 Project Structure

```
eazy-commerce-website/
├── 📁 public/                    # Static assets
│   ├── next.svg                  # Next.js logo
│   ├── vercel.svg               # Vercel logo  
│   └── ...                      # Other static files
├── 📁 src/
│   └── 📁 app/                  # Next.js App Router
│       ├── favicon.ico          # Website favicon
│       ├── globals.css          # Global styles & Tailwind imports
│       ├── layout.tsx           # Root layout component
│       └── page.tsx             # Homepage component
├── 📄 next.config.ts            # Next.js configuration
├── 📄 package.json              # Dependencies & scripts
├── 📄 postcss.config.mjs        # PostCSS configuration
├── 📄 tsconfig.json             # TypeScript configuration
└── 📄 README.md                 # Project documentation
```

## 🎯 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with Turbopack |
| `npm run build` | Build production-ready application |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint for code quality checks |

### Development Workflow

1. **Development**: `npm run dev` - Start with hot reloading
2. **Type Checking**: TypeScript will check types automatically
3. **Linting**: `npm run lint` - Check code quality
4. **Building**: `npm run build` - Create production build
5. **Testing**: `npm run start` - Test production build locally

## ⚙️ Configuration Details

### TypeScript Configuration
- **Strict mode enabled** for better type safety
- **Path aliases configured**: Use `@/*` to import from `src/*`
- **Modern ES2017 target** with latest library support
- **JSX preservation** for optimal Next.js integration

### Tailwind CSS Setup
- **Version 4.x** with improved performance
- **Dark mode support** via `prefers-color-scheme`
- **Custom CSS variables** for theming
- **PostCSS integration** for processing

### Next.js Features
- **App Router architecture** for modern routing
- **Turbopack development** for faster builds
- **Automatic font optimization** with Geist fonts
- **Image optimization** ready for e-commerce assets

## 🎨 Styling Guide

This project uses Tailwind CSS v4 with custom CSS variables for consistent theming:

### Color Scheme
```css
/* Light mode */
--background: #ffffff
--foreground: #171717

/* Dark mode (automatic) */
--background: #0a0a0a  
--foreground: #ededed
```

### Font Stack
- **Primary**: Geist Sans (optimized web font)
- **Monospace**: Geist Mono (for code elements)

## 📦 Adding Dependencies

### For UI Components
```bash
npm install @radix-ui/react-* # Accessible components
npm install lucide-react      # Modern icons
```

### For State Management
```bash
npm install zustand          # Lightweight state management
npm install @tanstack/react-query # Server state management
```

### For Forms & Validation
```bash
npm install react-hook-form  # Performance forms
npm install zod              # Schema validation
```

## 🚀 Deployment

### Deploy to Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Vercel will automatically deploy on every push

### Manual Deployment
```bash
npm run build    # Create production build
npm run start    # Start production server
```

### Environment Variables
Create a `.env.local` file for environment-specific variables:
```bash
# Database
DATABASE_URL="your-database-url"

# Authentication
NEXTAUTH_SECRET="your-secret-key"
NEXTAUTH_URL="http://localhost:3000"

# Payment Processing
STRIPE_SECRET_KEY="your-stripe-key"
```

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/your-feature`
3. **Follow code standards**: Use TypeScript, follow naming conventions
4. **Test your changes**: Ensure `npm run build` passes
5. **Commit changes**: Use conventional commit messages
6. **Submit a pull request**: Describe your changes clearly

### Code Standards
- Use **TypeScript** for all new files
- Follow **functional component** patterns
- Use **named exports** over default exports
- Implement **proper error handling**
- Write **descriptive variable names**
- Add **JSDoc comments** for complex functions

## 📚 Learning Resources

### Next.js Resources
- [Next.js Documentation](https://nextjs.org/docs) - Official documentation
- [Next.js 15 Features](https://nextjs.org/blog/next-15) - Latest features overview
- [App Router Guide](https://nextjs.org/docs/app) - Modern routing patterns

### React Resources  
- [React 19 Features](https://react.dev/blog/2024/04/25/react-19) - New React features
- [React Documentation](https://react.dev) - Official React docs

### TypeScript & Tailwind
- [TypeScript Handbook](https://www.typescriptlang.org/docs/) - TypeScript guide
- [Tailwind CSS v4](https://tailwindcss.com/docs) - Styling documentation

## 🐛 Troubleshooting

### Common Issues

**Build Errors**
```bash
rm -rf .next node_modules
npm install
npm run build
```

**Type Errors**
```bash
npx tsc --noEmit  # Check TypeScript errors
```

**Styling Issues**
```bash
# Ensure Tailwind is properly configured
npm run dev  # Restart development server
```

### Getting Help
- Check [Next.js GitHub Issues](https://github.com/vercel/next.js/issues)
- Visit [Next.js Discussions](https://github.com/vercel/next.js/discussions)
- Join [Vercel Discord](https://discord.gg/vercel)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Built with ❤️ using Next.js 15, React 19, and TypeScript**
