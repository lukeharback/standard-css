# Standard CSS

This tiny css library provides default styling and some small utilities.

## Features

- 🎨 **Design Tokens**: CSS custom properties for consistent theming
- 🌙 **Dark Mode**: Automatic dark mode support using `prefers-color-scheme`
- 📱 **Responsive**: Mobile-first approach with responsive utilities
- 🎯 **Utility-First**: Practical utility classes for common use cases
- ♿ **Accessible**: Focus states and semantic HTML support
- 🚀 **Lightweight**: Minimal footprint with maximum utility

## Installation

Download the files from the `src/` directory and include them in your HTML:

```html
<link rel="stylesheet" href="src/tokens.css">
<link rel="stylesheet" href="src/base.css">
<link rel="stylesheet" href="src/utility.css">
```

## Quick Start

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My App</title>
    <link rel="stylesheet" href="src/tokens.css">
    <link rel="stylesheet" href="src/base.css">
    <link rel="stylesheet" href="src/utility.css">
</head>
<body class="container-md m-auto">
    <header class="m-md">
        <h1>Welcome to Standard CSS</h1>
        <p class="text-callout">A lightweight CSS utility library</p>
    </header>

    <main class="m-md">
        <div class="card p-md">
            <h2>Getting Started</h2>
            <p>Start building with our utility classes and sensible defaults.</p>
            <button class="btn-primary">Get Started</button>
        </div>
    </main>
</body>
</html>
```

## Documentation

### Design Tokens

Standard CSS uses CSS custom properties for consistent theming:

```css
:root {
    /* Colors */
    --color-accent: #ff3366;
    --color-background-primary: #ffffff;
    --color-text-primary: #333333;

    /* Spacing */
    --sizing-xs: 4px;
    --sizing-sm: 8px;
    --sizing-md: 16px;
    --sizing-lg: 32px;

    /* Typography */
    --font-size: 0.875rem;
    --font-family: ui-sans-serif, system-ui, -apple-system, ...;
}
```

### Layout Utilities

#### Containers
- `.container-lg` - Large container (1200px max-width)
- `.container-md` - Medium container (840px max-width)

#### Flexbox
- `.flex` - Display flex
- `.flex-row` - Flex direction row
- `.flex-col` - Flex direction column
- `.flex-auto` - Responsive flex (row on desktop, column on mobile)
- `.flex-grow` - Flex grow 1
- `.flex-row-end` - Justify content end
- `.flex-row-space-between` - Justify content space-between
- `.flex-row-align-center` - Align items center

#### Grid
- `.grid` - CSS Grid with auto-fill columns

### Spacing Utilities

#### Margin
- `.m-auto` - Margin auto
- `.m-xs`, `.m-sm`, `.m-md`, `.m-lg` - All sides
- `.m-x-xs`, `.m-x-sm`, `.m-x-md`, `.m-x-lg` - Horizontal
- `.m-y-xs`, `.m-y-sm`, `.m-y-md`, `.m-y-lg` - Vertical

#### Padding
- `.p-xs`, `.p-sm`, `.p-md`, `.p-lg` - All sides
- `.p-x-xs`, `.p-x-sm`, `.p-x-md`, `.p-x-lg` - Horizontal
- `.p-y-xs`, `.p-y-sm`, `.p-y-md`, `.p-y-lg` - Vertical

### Typography Utilities

#### Text Alignment
- `.text-left` - Text align left
- `.text-center` - Text align center
- `.text-right` - Text align right
- `.text-justify` - Text align justify

#### Font Weight
- `.font-light` - Font weight 300
- `.font-normal` - Font weight 400
- `.font-medium` - Font weight 500
- `.font-semibold` - Font weight 600
- `.font-bold` - Font weight 700
- `.font-extrabold` - Font weight 800

### Display & Position

#### Display
- `.hidden` - Display none
- `.block` - Display block
- `.inline` - Display inline
- `.inline-block` - Display inline-block
- `.flex` - Display flex
- `.grid` - Display grid

#### Position
- `.relative` - Position relative
- `.absolute` - Position absolute
- `.fixed` - Position fixed
- `.sticky` - Position sticky

#### Z-Index
- `.z-0`, `.z-10`, `.z-20`, `.z-30`, `.z-40`, `.z-50` - Z-index values

### Border & Shadow

#### Borders
- `.border` - Border all sides
- `.border-0` - No border
- `.border-t`, `.border-r`, `.border-b`, `.border-l` - Individual sides
- `.border-radius`, `.border-radius-sm`, `.border-radius-md`, `.border-radius-lg`, `.border-radius-full` - Border radius

#### Shadows
- `.shadow-sm` - Small shadow
- `.shadow` - Default shadow
- `.shadow-md` - Medium shadow
- `.shadow-lg` - Large shadow
- `.shadow-xl` - Extra large shadow
- `.shadow-none` - No shadow

### Components

#### Buttons
- `.btn` - Default button
- `.btn-primary` - Primary button
- `.btn-secondary` - Secondary button

#### Cards
- `.card` - Card component with background and border

#### Alerts
- `.alert` - Success alert
- `.alert-error` - Error alert

### Responsive Utilities

Use responsive prefixes for different breakpoints:

- `sm:` - Small screens (max-width: 576px)
- `md:` - Medium screens (min-width: 768px)
- `lg:` - Large screens (min-width: 992px)

Example:
```html
<div class="hidden md:block">Hidden on mobile, visible on desktop</div>
<div class="text-center lg:text-left">Centered on mobile, left-aligned on desktop</div>
```

## Dark Mode

Standard CSS automatically supports dark mode using the `prefers-color-scheme` media query. All components and utilities automatically adapt to dark mode when the user's system preference is set to dark.

## Customization

You can customize the design tokens by overriding CSS custom properties:

```css
:root {
    --color-accent: #your-brand-color;
    --font-family: 'Your Custom Font', sans-serif;
    --sizing-md: 20px;
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Demo

View the [demo page](demo.html) to see all components and utilities in action.

