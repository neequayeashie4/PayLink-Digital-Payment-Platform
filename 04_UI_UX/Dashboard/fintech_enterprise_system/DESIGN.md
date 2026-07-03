---
name: Fintech Enterprise System
colors:
  surface: '#fbf8ff'
  surface-dim: '#dcd9e0'
  surface-bright: '#fbf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f2fa'
  surface-container: '#f0ecf4'
  surface-container-high: '#eae7ee'
  surface-container-highest: '#e4e1e9'
  on-surface: '#1b1b20'
  on-surface-variant: '#464651'
  inverse-surface: '#303035'
  inverse-on-surface: '#f3eff7'
  outline: '#777682'
  outline-variant: '#c7c5d3'
  surface-tint: '#5157a5'
  primary: '#121666'
  on-primary: '#ffffff'
  primary-container: '#2a2f7c'
  on-primary-container: '#959bee'
  inverse-primary: '#bfc2ff'
  secondary: '#006c4b'
  on-secondary: '#ffffff'
  secondary-container: '#60f9bd'
  on-secondary-container: '#00714f'
  tertiary: '#4e000a'
  on-tertiary: '#ffffff'
  tertiary-container: '#770014'
  on-tertiary-container: '#ff7777'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e0e0ff'
  primary-fixed-dim: '#bfc2ff'
  on-primary-fixed: '#080b60'
  on-primary-fixed-variant: '#393e8b'
  secondary-fixed: '#63fcc0'
  secondary-fixed-dim: '#3fdfa5'
  on-secondary-fixed: '#002114'
  on-secondary-fixed-variant: '#005138'
  tertiary-fixed: '#ffdad8'
  tertiary-fixed-dim: '#ffb3b0'
  on-tertiary-fixed: '#410007'
  on-tertiary-fixed-variant: '#92001b'
  background: '#fbf8ff'
  on-background: '#1b1b20'
  surface-variant: '#e4e1e9'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  '4': 4px
  '8': 8px
  '12': 12px
  '16': 16px
  '24': 24px
  '32': 32px
  '40': 40px
  '48': 48px
  '64': 64px
  '80': 80px
---

## Brand & Style
The design system is engineered for high-stakes financial operations, prioritizing clarity, institutional trust, and high-density information management. Drawing inspiration from modern neo-corporate aesthetics, the style is **Corporate / Modern** with a focus on precision and efficiency.

The visual narrative balances a heavy indigo primary foundation with vast amounts of "breathing room" (off-white whitespace) to reduce cognitive load during complex tasks. The interface feels premium and technical, utilizing subtle depth and sharp geometric forms to create a structured environment where financial data remains the hero. It is designed to evoke a sense of absolute reliability and forward-thinking professionalism.

## Colors
The palette is rooted in a deep Indigo primary, signaling authority and stability. Semantic colors—Teal (Success), Coral (Danger), and Amber (Warning)—are calibrated for high visibility against both white surfaces and the off-white background. 

- **Primary Indigo:** Used for main actions, navigation states, and brand-heavy components.
- **Surface & Background:** A strict distinction is maintained between the `#F7F8FA` page background and `#FFFFFF` component surfaces to create natural grouping through tonal contrast.
- **Data Visualization:** Tabular data should use the neutral slate for headers and the primary text color for values to ensure maximum legibility.

## Typography
This design system utilizes **Inter** for its neutral, highly legible characteristics. A critical requirement for this fintech environment is the use of **Tabular Figures** (`tnum`) for all numerical data, ensuring that currency values and transaction amounts align perfectly in tables and dashboards.

- **Scale:** A tight scale is used for body content to allow for information density.
- **Hierarchy:** Use `label-caps` for table headers and section overviews.
- **Weight:** Reserve 700 weight for display titles and 600 for sub-headers. Body text should remain at 400 for optimal long-form reading.

## Layout & Spacing
The system follows a strict **8pt Grid** to ensure mathematical harmony across all components. 

- **Grid System:** A 12-column fluid grid is used for desktop layouts, transitioning to a 4-column layout for mobile devices.
- **Density:** For data-heavy views (like transaction ledgers), the 4px and 8px units should be used for internal component padding to maximize content visibility. 
- **Structure:** Use 24px gutters to provide clear separation between dashboard widgets and 32px-48px for vertical section spacing.

## Elevation & Depth
Depth is used sparingly to maintain a clean, professional "flat-plus" aesthetic. Hierarchy is primarily established through tonal layering, with shadows reserved for specific interaction cues.

- **Level 1 (Flat):** Used for the main background.
- **Level 2 (Cards):** Soft, ambient shadow using `0px 4px 20px rgba(26, 26, 46, 0.05)`. This elevates primary containers and dashboard widgets from the off-white background.
- **Level 3 (Overlays):** Used for dropdowns, tooltips, and modals. A more pronounced shadow using `0px 8px 32px rgba(26, 26, 46, 0.12)` provides clear focus for temporary UI elements.

## Shapes
The shape language is sophisticated and approachable, moving away from sharp industrial corners toward more organic, rounded geometry. 

- **Cards:** Use a generous 18px radius to frame dashboard content comfortably.
- **Interactions:** Buttons utilize a 12px radius, providing a distinct "tap" target feel that differentiates them from inputs (8px).
- **Charts:** All data visualizations and progress bars should use a 16px radius for a modern, fluid appearance.

## Components

### Buttons
Primary buttons use the Indigo background with White text and a 12px radius. Secondary buttons should use a ghost style (Indigo border and text) or a light wash of the primary color.

### Cards
Cards are the primary container for the system. They must feature the 18px corner radius, a white surface, and the Level 2 subtle shadow. Internal padding should default to 24px.

### Inputs & Fields
Input fields use a 1px border (`#EAEAF0`) and an 8px radius. When focused, the border shifts to the Primary Indigo with a 2px outer glow of the same color at 10% opacity.

### Data Tables
Tables should have no outer borders, using only horizontal dividers in `#EAEAF0`. Row hover states should use the `#F7F8FA` background color. Column headers use `label-caps` typography.

### Chips & Status Indicators
Status chips use a "light" version of the semantic colors (e.g., 10% opacity Teal background with 100% opacity Teal text) to indicate transaction states like 'Completed', 'Pending', or 'Failed'. Use a pill-shaped (full) radius.

### Charts
Financial charts should utilize the Teal and Indigo palette. Line charts should use a stroke width of 2px or 3px with smoothed (rounded) joints to match the system's shape language.