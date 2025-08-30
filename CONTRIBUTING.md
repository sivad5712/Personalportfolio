
# Contributing to Siva D Portfolio

Thank you for your interest in contributing to this portfolio project! This document provides guidelines for contributing.

## 🚀 Getting Started

### Prerequisites
- Node.js 18.0 or higher
- npm or yarn package manager
- Git

### Development Setup
1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/yourusername/siva-portfolio.git
   ```
3. Install dependencies:
   ```bash
   cd siva-portfolio/app
   yarn install
   ```
4. Start development server:
   ```bash
   yarn dev
   ```

## 🛠️ Development Guidelines

### Code Style
- Use **TypeScript** for all new code
- Follow **ESLint** and **Prettier** configurations
- Use **Tailwind CSS** for styling
- Write **meaningful component names** and **clear comments**

### Component Structure
```typescript
// Component template
'use client';

import { motion } from 'framer-motion';
import { useInView } from 'react-intersection-observer';

export default function ComponentName() {
  const [ref, inView] = useInView({
    triggerOnce: true,
    threshold: 0.1
  });

  return (
    <section id="section-id" className="py-20">
      {/* Component content */}
    </section>
  );
}
```

### Commit Messages
Use conventional commit format:
- `feat:` new features
- `fix:` bug fixes
- `docs:` documentation changes
- `style:` formatting changes
- `refactor:` code refactoring
- `test:` adding tests
- `chore:` maintenance tasks

Example:
```bash
git commit -m "feat: add new skills section animation"
```

## 📝 Making Changes

### 1. Content Updates
- Update personal information in `lib/data.ts`
- Add new projects, experience, or skills
- Modify certification details

### 2. Design Changes
- Update global styles in `app/globals.css`
- Modify component styling with Tailwind classes
- Add new animations using Framer Motion

### 3. Feature Additions
- Create new components in `components/`
- Add to main page in `app/page.tsx`
- Update navigation if needed

## 🧪 Testing

### Before Submitting
1. **Build successfully**: `yarn build`
2. **No TypeScript errors**: `yarn type-check`
3. **ESLint passes**: `yarn lint`
4. **Manual testing**: Test on desktop and mobile

### Testing Checklist
- [ ] All sections load correctly
- [ ] Animations work smoothly
- [ ] Responsive design on all devices
- [ ] Navigation links work properly
- [ ] Contact links function correctly
- [ ] No console errors

## 📦 Pull Request Process

1. **Create feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** following the guidelines

3. **Test thoroughly** using the testing checklist

4. **Commit your changes**:
   ```bash
   git add .
   git commit -m "feat: your descriptive commit message"
   ```

5. **Push to your fork**:
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create Pull Request** on GitHub with:
   - Clear description of changes
   - Screenshots if UI changes
   - Testing notes

## 🐛 Bug Reports

When reporting bugs, please include:
- **Description** of the issue
- **Steps to reproduce**
- **Expected behavior**
- **Actual behavior**
- **Browser/device information**
- **Screenshots** if applicable

## 💡 Feature Requests

For new features:
- **Describe the feature** clearly
- **Explain the use case**
- **Provide mockups** if applicable
- **Consider implementation complexity**

## 📋 Code Review Criteria

- ✅ Code follows TypeScript best practices
- ✅ Components are properly typed
- ✅ Responsive design maintained
- ✅ Accessibility guidelines followed
- ✅ Performance considerations addressed
- ✅ No breaking changes to existing functionality

## 🎨 Design Guidelines

### UI Consistency
- Use existing color palette and design tokens
- Maintain consistent spacing using Tailwind utilities
- Follow established component patterns
- Ensure proper contrast ratios for accessibility

### Animation Guidelines
- Use Framer Motion for consistency
- Keep animations subtle and purposeful
- Ensure animations don't cause motion sickness
- Test performance on lower-end devices

## 🔗 Useful Resources

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Framer Motion Documentation](https://www.framer.com/motion/)
- [Radix UI Documentation](https://www.radix-ui.com/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)

## 📞 Questions?

If you have questions about contributing:
- Open an issue for discussion
- Reach out via email: siva.d@example.com
- Check existing issues and discussions

---

**Thank you for contributing to make this portfolio even better! 🙏**
