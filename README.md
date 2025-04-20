# MiniCSS

A lightweight CSS framework with light and dark mode support, built with SASS.

## Features

- Light and dark mode support
- Responsive design
- Semantic HTML styling
- Form elements styling
- Typography and spacing utilities
- Small file size
- Easy to customize

## Installation

### NPM

```bash
npm install minicss
```

### CDN

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/minicss@latest/css/minicss.min.css">
```

### Manual

1. Download the latest release
2. Include `minicss.css` in your HTML file:
```html
<link rel="stylesheet" href="path/to/minicss.css">
```

## Usage

### Basic Setup

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <link rel="stylesheet" href="minicss.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>My Website</h1>
        </header>
        <main>
            <p>Hello, world!</p>
        </main>
        <footer>
            <p>© 2025</p>
        </footer>
    </div>
</body>
</html>
```

### Dark Mode

MiniCSS supports dark mode through the `data-theme` attribute:

```html
<html data-theme="dark">
```

To toggle between themes, you can use JavaScript:

```javascript
function toggleTheme() {
    const html = document.documentElement;
    const currentTheme = html.getAttribute('data-theme');
    const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
    html.setAttribute('data-theme', newTheme);
}
```

### Container

Use the `.container` class for a responsive container:

```html
<div class="container">
    <!-- Your content -->
</div>
```

### Grid

Use the `.grid` class for a responsive grid layout:

```html
<div class="grid">
    <div>Column 1</div>
    <div>Column 2</div>
    <div>Column 3</div>
</div>
```

### Spacing Utilities

MiniCSS includes margin and padding utilities:

```html
<div class="m-1">Small margin</div>
<div class="p-2">Medium padding</div>
```

Available classes:
- `m-0` to `m-5` for margin
- `mt-0` to `mt-5` for margin-top
- `mr-0` to `mr-5` for margin-right
- `mb-0` to `mb-5` for margin-bottom
- `ml-0` to `ml-5` for margin-left
- `p-0` to `p-5` for padding
- `pt-0` to `pt-5` for padding-top
- `pr-0` to `pr-5` for padding-right
- `pb-0` to `pb-5` for padding-bottom
- `pl-0` to `pl-5` for padding-left

### Responsive Utilities

Hide elements on different screen sizes:

```html
<div class="hidden-sm">Hidden on small screens</div>
<div class="hidden-md">Hidden on medium screens</div>
<div class="hidden-lg">Hidden on large screens</div>
<div class="hidden-xl">Hidden on extra large screens</div>
```

## Development

1. Clone the repository
2. Install dependencies:
```bash
npm install
```
3. Start development server:
```bash
npm run dev
```
4. Build for production:
```bash
npm run build
```

## License

MIT 