# Tech Stack & Environment Configuration

## Core Technology Stack
- **Frontend / Client**: [e.g., React 19, Vite, TypeScript, TailwindCSS v4]
- **Backend / API**: [e.g., Node.js with Express, Python FastAPI, or None]
- **Database / Storage**: [e.g., PostgreSQL, SQLite, LocalStorage]
- **State Management**: [e.g., Zustand, Redux Toolkit, Context API]

## Development Toolchain & Commands
- **Package Manager**: [e.g., npm / pnpm / yarn]
- **Install Dependencies**: `[e.g., npm install]`
- **Run Development Server**: `[e.g., npm run dev]`
- **Production Build**: `[e.g., npm run build]`
- **Linting & Formatting**: `[e.g., npm run lint]`

## Configuration Files to Protect
*Do not alter these files without verifying breaking changes:*
- `package.json`
- `tsconfig.json`
- `vite.config.ts`

## Technical Constraints & Guidelines
1. **Type Safety**: Absolute strict TypeScript compliance. No use of `any`.
2. **Styling Rules**: Maintain component isolation using utility classes or scoped modules.
3. **Environment**: App must compile with standard web browser compatibility (no specific Node APIs in frontend).
