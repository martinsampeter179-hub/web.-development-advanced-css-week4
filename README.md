SpendWise — Personal Finance Dashboard Shell

A responsive, accessible personal finance dashboard layout built with semantic HTML5, CSS Grid, and Flexbox for the Week 4 CSS Layout Challenge.

Features & Implementation Breakdown

1. Modern Dashboard Architecture

CSS Grid Page Frame: Uses grid-template-areas to divide the screen into a distinct Sidebar, Header, and Main Content region without using absolute positioning.

Component-Level Flexbox: Uses Flexbox inside individual UI components to handle alignment for navigation items, header search, user profile avatars, and card details.

2. Custom Property Theming & Dark Mode

Defined inside :root using CSS custom properties for uniform color management:

--brand-color (#2563eb): Used for branding, active states, and focus borders.

--accent-color (#059669): Highlights financial totals and metric figures.

--surface-bg, --card-bg: Handles background surface contrast.

--text-primary, --text-secondary: Ensures readable text hierarchy.

Dark Theme Support: Includes @media (prefers-color-scheme: dark) overrides to automatically switch theme variables based on system settings.

3. Micro-Interactions & Accessibility

Dashboard cards include smooth 200ms transitions (transform: translateY(-4px) and box-shadow) triggered on both :hover and :focus-visible keyboard focus states.

Form inputs and card containers feature accessible focus outlines for enhanced navigation.

4. Responsive Breakpoint

Below 768px, a @media query re-configures the grid into a single-column layout, moving navigation to a horizontal scroll menu and stacking content cards cleanly.

File Structure

spendwise-dashboard/
├── index.html    # Main dashboard semantic layout
├── style.css     # CSS Grid, Flexbox styles, theme variables, and media queries
└── README.md     # Project documentation
