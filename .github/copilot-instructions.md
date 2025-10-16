# Copilot Instructions for prismarc-site

## Project Overview
- This is a Next.js project using the `/src/app` directory structure and TypeScript.
- UI components are organized under `src/app/components/ui/`.
- Utility functions live in `src/app/lib/utils.ts`.
- Global styles and theme variables are managed in `src/app/globals.css`.

## Key Patterns & Conventions
- **Component Structure:**
  - Use functional React components with TypeScript.
  - UI components (e.g., `button.tsx`, `card.tsx`) are colocated in `src/app/components/ui/`.
  - Pages are defined in `src/app/[route]/page.tsx` (e.g., `about/page.tsx`).
- **Styling:**
  - Tailwind CSS is used for utility-first styling. Custom properties and theme variables are defined in `globals.css`.
  - Use `@apply` for base styles and reference CSS variables for colors and radii.
  - Dark mode is handled via the `.dark` class and custom properties.
- **Imports:**
  - Prefer absolute imports from `src/app/` for internal modules.
- **Font Management:**
  - Uses `next/font` for optimized font loading (Geist font family).

## Developer Workflows
- **Development:**
  - Start the dev server: `npm run dev` (or `yarn dev`, `pnpm dev`, `bun dev`).
  - Edit pages in `src/app/[route]/page.tsx` and components in `src/app/components/ui/`.
- **Styling:**
  - Edit `globals.css` for theme and base style changes.
  - Use Tailwind utility classes in JSX, and custom properties for theme consistency.
- **Adding Components:**
  - Place new UI components in `src/app/components/ui/`.
  - Export components for use in pages or other components.
- **Utilities:**
  - Add shared logic to `src/app/lib/utils.ts`.

## External Integrations
- Tailwind CSS and `tw-animate-css` are imported in `globals.css`.
- No custom API or backend integration is present by default.

## Examples
- To create a new page, add a folder under `src/app/` (e.g., `blog/`) and a `page.tsx` file inside it.
- To add a new button variant, extend `button.tsx` in `components/ui/` and update styles in `globals.css` if needed.

## References
- See `README.md` for basic setup and deployment instructions.
- Review `globals.css` for theme and style conventions.
- Check `src/app/components/ui/` for reusable UI patterns.

---

_If any conventions or workflows are unclear, please ask for clarification or examples from the codebase._
