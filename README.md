
# 🚀 Portfolio Website

A modern, responsive portfolio website built with **Next.js 14**, **TypeScript**, and **Tailwind CSS**. This portfolio showcases professional experience, technical skills, certifications, and featured projects with an elegant dark theme and smooth animations.

![Portfolio Preview](https://img.shields.io/badge/Status-Production%20Ready-brightgreen) ![Next.js](https://img.shields.io/badge/Next.js-14-black) ![TypeScript](https://img.shields.io/badge/TypeScript-5.2-blue) ![Tailwind](https://img.shields.io/badge/Tailwind-3.3-38bdf8)

## ✨ Features

- 🎨 **Modern Dark Theme** with gradient backgrounds and glassmorphism effects
- 📱 **Fully Responsive** design optimized for desktop, tablet, and mobile
- ⚡ **Interactive Animations** using Framer Motion for smooth user experience
- 🛠️ **Technical Skills** visualization with animated progress bars
- 📊 **Project Showcase** with filtering (Personal/Professional projects)
- 💼 **Professional Experience** section with detailed achievements
- 🏆 **Certifications** display with official badges
- 📧 **Contact Integration** with direct email and social media links
- 🔍 **SEO Optimized** with proper meta tags and structured data
- ⚙️ **Performance Optimized** with Next.js Image optimization and lazy loading

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Framework** | Next.js 14 (App Router) |
| **Language** | TypeScript 5.2 |
| **Styling** | Tailwind CSS 3.3 |
| **UI Components** | Radix UI, Shadcn/ui |
| **Animations** | Framer Motion |
| **Icons** | Lucide React |
| **Theme** | next-themes |
| **Build Tool** | Webpack 5 |

## 📦 Installation & Setup

### Prerequisites
- **Node.js** 18.0 or higher
- **npm** or **yarn** package manager

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/siva-portfolio.git
cd siva-portfolio
```

### 2. Install Dependencies
```bash
# Using npm
npm install

# Or using yarn (recommended)
yarn install
```

### 3. Run Development Server
```bash
# Using npm
npm run dev

# Or using yarn
yarn dev
```

### 4. Open in Browser
Navigate to [http://localhost:3000](http://localhost:3000) to see the portfolio.

## 🏗️ Build & Deploy

### Local Production Build
```bash
# Build the application
npm run build

# Start production server
npm start
```

### Deploy to Vercel 
1. Push your code to GitHub
2. Connect your GitHub repository to [Vercel](https://vercel.com)
3. Deploy with zero configuration

[![Deploy with Vercel](https://i.ytimg.com/vi/CNJkX9rYI8U/mqdefault.jpg)


### Deploy to GitHub Pages
1. Update `next.config.js` with `output: 'export'`
2. Build: `npm run build`
3. Push the `out` folder to `gh-pages` branch

## 📁 Project Structure

```
app/
├── 📄 README.md                     # Project documentation
├── 📄 .gitignore                   # Git ignore rules
├── 📄 package.json                 # Dependencies and scripts
├── 📄 next.config.js               # Next.js configuration
├── 📄 tailwind.config.ts           # Tailwind CSS configuration
├── 📄 tsconfig.json                # TypeScript configuration
├── 📄 postcss.config.js            # PostCSS configuration
├── 📄 components.json              # Shadcn UI configuration
├── 📄 next-env.d.ts                # Next.js type definitions
├── 📁 app/
│   ├── 📄 layout.tsx               # Root layout component
│   ├── 📄 page.tsx                 # Home page
│   └── 📄 globals.css              # Global styles and CSS variables
├── 📁 components/
│   ├── 📄 navigation.tsx           # Navigation bar with smooth scroll
│   ├── 📄 hero-section.tsx         # Landing hero section
│   ├── 📄 about-section.tsx        # About me section
│   ├── 📄 certifications-section.tsx # Certifications display
│   ├── 📄 skills-section.tsx       # Technical skills with progress bars
│   ├── 📄 projects-section.tsx     # Projects showcase with filtering
│   ├── 📄 experience-section.tsx   # Professional experience
│   ├── 📄 theme-provider.tsx       # Theme context provider
│   └── 📁 ui/                      # Reusable UI components (40+ files)
├── 📁 lib/
│   ├── 📄 data.ts                  # Portfolio content and data
│   ├── 📄 types.ts                 # TypeScript type definitions
│   └── 📄 utils.ts                 # Utility functions
└── 📁 hooks/
    └── 📄 use-toast.ts             # Toast notification hook
```

## 🎨 Customization Guide

### Update Personal Information
Edit the content in `lib/data.ts`:

```typescript
// Update personal information
export const aboutMe = {
  title: "About Me",
  description: "Your bio here...",
  // ... rest of your data
};

// Update work experience
export const workExperience: Experience[] = [
  {
    title: "Your Job Title",
    company: "Company Name",
    // ... rest of experience data
  }
];
```

### Modify Colors & Styling
Update CSS variables in `app/globals.css`:

```css
:root {
  --primary: 217.2 91.2% 59.8%;    /* Blue theme */
  --background: 222.2 84% 4.9%;    /* Dark background */
  /* ... other color variables */
}
```

### Add New Sections
1. Create new component in `components/`
2. Import and add to `app/page.tsx`
3. Update navigation in `components/navigation.tsx`

## 🆚 VS Code Extensions (Essential)

### **Required Extensions:**
```json
{
  "recommendations": [
    "ms-vscode.vscode-typescript-next",
    "bradlc.vscode-tailwindcss",
    "esbenp.prettier-vscode",
    "ms-vscode.vscode-eslint",
    "formulahendry.auto-rename-tag",
    "christian-kohler.path-intellisense"
  ]
}
```

### **Extension Details:**

1. **ES7+ React/Redux/React-Native snippets** (`dsznajder.es7-react-js-snippets`)
   - React code snippets and shortcuts

2. **Tailwind CSS IntelliSense** (`bradlc.vscode-tailwindcss`)
   - Autocomplete for Tailwind classes

3. **TypeScript Importer** (`pmneo.tsimporter`)
   - Auto import TypeScript modules

4. **Prettier - Code formatter** (`esbenp.prettier-vscode`)
   - Code formatting

5. **ESLint** (`ms-vscode.vscode-eslint`)
   - Code linting and error detection

6. **Auto Rename Tag** (`formulahendry.auto-rename-tag`)
   - Automatically rename paired HTML/JSX tags

7. **Path Intellisense** (`christian-kohler.path-intellisense`)
   - File path autocomplete

8. **Next.js snippets** (`PulkitGangwar.nextjs-snippets`)
   - Next.js specific code snippets

### **Optional but Helpful:**
- **Thunder Client** (`rangav.vscode-thunder-client`) - API testing
- **GitLens** (`eamodio.gitlens`) - Enhanced Git capabilities
- **Auto Close Tag** (`formulahendry.auto-close-tag`) - Auto close HTML tags
- **Bracket Pair Colorizer** (`coenraads.bracket-pair-colorizer`) - Color matching brackets

## ⚙️ VS Code Settings

Create `.vscode/settings.json` in your project:

```json
{
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "typescript.preferences.importModuleSpecifier": "relative",
  "emmet.includeLanguages": {
    "typescript": "html",
    "typescriptreact": "html"
  },
  "tailwindCSS.includeLanguages": {
    "typescript": "html",
    "typescriptreact": "html"
  }
}
```

## 🚀 GitHub Upload Steps

### **Method 1: Command Line**
```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Siva D Portfolio"

# Add remote repository
git remote add origin https://github.com/yourusername/siva-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### **Method 2: GitHub Desktop**
1. Download **GitHub Desktop**
2. Clone/Create new repository
3. Copy all files to repository folder
4. Commit and push changes

### **Method 3: VS Code Git Integration**
1. Open project in VS Code
2. Initialize repository (Source Control panel)
3. Stage all changes
4. Commit with message
5. Publish to GitHub

## 🔧 Development Workflow

### **1. Local Development**
```bash
yarn dev          # Start development server
yarn build        # Build for production
yarn start        # Start production server
yarn lint         # Run ESLint
```

### **2. Code Quality**
- **ESLint** for code linting
- **Prettier** for code formatting
- **TypeScript** for type safety
- **Tailwind** for consistent styling

### **3. Git Workflow**
```bash
git checkout -b feature/new-section    # Create feature branch
# Make changes
git add .
git commit -m "Add new portfolio section"
git push origin feature/new-section
# Create pull request on GitHub
```

## 🌐 Environment Variables

Create `.env.local` for development:

```env
# Optional: Analytics
NEXT_PUBLIC_GA_ID=your-google-analytics-id

# Optional: Contact Form
NEXT_PUBLIC_CONTACT_EMAIL=your-email@example.com

# Optional: Social Links
NEXT_PUBLIC_LINKEDIN_URL=https://linkedin.com/in/your-profile
NEXT_PUBLIC_GITHUB_URL=https://github.com/your-username
```

## 📊 Performance Features

- ⚡ **Next.js Image Optimization** for faster loading
- 🎯 **Code Splitting** for optimal bundle sizes
- 📱 **Progressive Web App** ready
- 🔍 **SEO Optimized** with meta tags and structured data
- 🎨 **CSS-in-JS** with Tailwind for better performance

## 🎯 SEO Features

- ✅ Proper HTML semantic structure
- ✅ Meta tags for social media sharing
- ✅ Open Graph protocol implementation
- ✅ Twitter Card support
- ✅ Structured data for better search indexing
- ✅ Sitemap generation ready

## 📱 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)




## 📞 Contact & Support

- **💼 LinkedIn**: [linkedin.com/in/siva-d](https://linkedin.com/in/siva-d)
- **🐙 GitHub**: [github.com/siva-d](https://github.com/siva-d)

**🔥 Built with passion by Siva D - Sr. Software Engineer**

