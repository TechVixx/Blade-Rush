# AI Rules

## Tech stack

- Build the application with **React** and **TypeScript**.
- Use **React Router** for client-side navigation; keep all route definitions in `src/App.tsx`.
- Use **Tailwind CSS** for styling, layout, spacing, responsive behavior, colors, and states.
- Use **shadcn/ui** components as the default UI foundation.
- Use the installed **Radix UI** primitives through shadcn/ui when accessible, composable interactions are needed.
- Use **lucide-react** for icons instead of drawing custom SVG icons or adding another icon library.
- Keep application source code inside `src/`.
- Put route-level pages in `src/pages/` and reusable UI in `src/components/`.
- Use `src/pages/Index.tsx` as the default page and update it whenever new components need to appear in the main experience.

## Library and implementation rules

- Prefer existing shadcn/ui components for buttons, inputs, dialogs, menus, cards, tabs, forms, and other common UI patterns before creating custom equivalents.
- Use Tailwind utility classes directly in React components; do not introduce a separate styling system or scattered inline styles unless a value cannot reasonably be expressed with Tailwind.
- Use Radix UI primitives only through existing shadcn/ui components or when a shadcn/ui component does not cover the interaction.
- Use lucide-react icons consistently, with accessible labels or accompanying text when an icon-only control is not self-explanatory.
- Use React Router links and navigation APIs for in-app navigation; do not use raw anchors for internal routes.
- Keep pages focused on route composition and move reusable sections, controls, and visual patterns into `src/components/`.
- Keep types explicit at public component boundaries and avoid introducing `any` when a meaningful TypeScript type can be used.
- Reuse existing dependencies and project conventions; do not add a new library when React, Tailwind CSS, shadcn/ui, Radix UI, or lucide-react already solves the need.
- Preserve accessible semantics, keyboard interaction, visible focus states, and responsive behavior in every UI change.
