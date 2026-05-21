## 🚀 Comment l'utiliser concrètement dans l'interface Graphique (Desktop) ?
**1- À l'ouverture du projet :**
    Ouvrez votre dossier dans l'application de bureau OpenCode. Dans la zone de chat de votre projet actuel, saisissez simplement initialize memory bank si le dossier .memory-bank/ n'existe pas encore. L'IA va scanner vos fichiers en arrière-plan et générer la documentation technique automatiquement.

**2- Lors des changements de Sessions/Threads :**
    Si vous ouvrez un nouvel onglet ou créez un nouveau thread dans l'interface graphique pour travailler sur un autre aspect du projet, l'IA chargera instantanément le fichier AGENTS.md et affichera le tag de validation : [Memory Bank: Active] ....

**3- Persistance :** 
    Avant de fermer l'application à la fin de votre journée de développement, écrivez simplement update memory bank dans le chat. L'assistant écrira les dernières avancées dans votre dossier local. Vous pourrez ainsi fermer l'application en toute sécurité.



📦 1. Le modèle technique (.memory-bank/tech.md)Ce fichier indique à OpenCode l'environnement dans lequel il doit travailler, évitant qu'il n'invente des packages incompatibles ou n'utilise les mauvaises commandes de build.


📋 2. Le modèle de routines (.memory-bank/tasks.md)Ce fichier sert de guide de référence pour OpenCode lorsqu'il doit répéter une action à plusieurs reprises dans le projet. Vous pouvez y ajouter vos propres workflows au fil du temps.

Voici les structures de base pour vos deux fichiers. Vous pouvez copier directement ces modèles de code dans leurs fichiers respectifs au sein du dossier .memory-bank/.
Ces squelettes sont conçus pour être clairs, structurés et facilement interprétables par l'application Desktop d'OpenCode.
------------------------------
## 📦 1. Le modèle technique (.memory-bank/tech.md)
Ce fichier indique à OpenCode l'environnement dans lequel il doit travailler, évitant qu'il n'invente des packages incompatibles ou n'utilise les mauvaises commandes de build.

# Tech Stack & Environment Configuration## Core Technology Stack- **Frontend / Client**: [e.g., React 18, Vite, TypeScript, TailwindCSS]
- **Backend / API**: [e.g., Node.js with Express, Python FastAPI, or None]
- **Database / Storage**: [e.g., PostgreSQL, SQLite, LocalStorage]
- **State Management**: [e.g., Zustand, Redux Toolkit, Context API]
## Development Toolchain & Commands- **Package Manager**: [e.g., npm / pnpm / yarn]
- **Install Dependencies**: `[e.g., npm install]`
- **Run Development Server**: `[e.g., npm run dev]`
- **Production Build**: `[e.g., npm run build]`
- **Linting & Formatting**: `[e.g., npm run lint]`
## Configuration Files to Protect*Do not alter these files without verifying breaking changes:*
- `package.json`
- `tsconfig.json`
- `vite.config.ts`
## Technical Constraints & Guidelines1. **Type Safety**: Absolute strict TypeScript compliance. No use of `any`.2. **Styling Rules**: Maintain component isolation using utility classes or scoped modules.3. **Environment**: App must compile with standard web browser compatibility (no specific Node APIs in frontend).

------------------------------
## 📋 2. Le modèle de routines (.memory-bank/tasks.md)
Ce fichier sert de guide de référence pour OpenCode lorsqu'il doit répéter une action à plusieurs reprises dans le projet. Vous pouvez y ajouter vos propres workflows au fil du temps.

# Technical Task Runbooks
This file documents step-by-step engineering workflows for repetitive patterns in this project to prevent regressions and enforce architectural consistency.
---
## Template: [Task Name Example: Adding a New Component]
**Status:** Ready / Standardized
### Target Files to Create / Modify:- `/src/components/[ComponentName]/[ComponentName].tsx` - Create component
- `/src/components/[ComponentName]/index.ts` - Export interface
- `/src/components/index.ts` - Register globally if needed
### Verification Checklist:- [ ] Component is fully responsive using flexbox/grid.
- [ ] Types are cleanly exported.
- [ ] Component is tested locally inside OpenCode live previews.
### Execution Workflow Sequence:1. **Scaffold**: Create a directory with the component name inside the matching domain folder.
2. **Implement**: Code the structural JSX/TSX and apply the standardized design patterns defined in `architecture.md`.3. **Export**: Expose the component through the local folder index file to clean up root imports.

------------------------------
## 🎯 Prochaine étape logique
Maintenant que vos fichiers structurels sont prêts dans votre projet :

   1. Lancez votre application de bureau OpenCode.
   2. Écrivez simplement : initialize memory bank dans le chat de l'application.

L'IA va automatiquement lire ces deux modèles, inspecter le reste de votre code source, puis remplacer les données entre crochets [...] par les vraies technologies et dossiers de votre application.

Souhaitez-vous que nous passions à l'écriture du fichier architecture.md pour lui expliquer l'arborescence de votre code, ou préférez-vous lancer l'initialisation directement ?

