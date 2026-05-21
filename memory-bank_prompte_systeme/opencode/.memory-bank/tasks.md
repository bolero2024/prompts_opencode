# Technical Task Runbooks

This file documents step-by-step engineering workflows for repetitive patterns in this project to prevent regressions and enforce architectural consistency.

---

## Template: [Task Name Example: Adding a New Component]
**Status:** Ready / Standardized

### Target Files to Create / Modify:
- `/src/components/[ComponentName]/[ComponentName].tsx` - Create component
- `/src/components/[ComponentName]/index.ts` - Export interface
- `/src/components/index.ts` - Register globally if needed

### Verification Checklist:
- [ ] Component is fully responsive using flexbox/grid.
- [ ] Types are cleanly exported.
- [ ] Component is tested locally inside OpenCode live previews.

### Execution Workflow Sequence:
1. **Scaffold**: Create a directory with the component name inside the matching domain folder.
2. **Implement**: Code the structural JSX/TSX and apply the standardized design patterns defined in `architecture.md`.
3. **Export**: Expose the component through the local folder index file to clean up root imports.
