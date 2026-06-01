## Using Google Material Symbols Icons

This project uses **Google Material Symbols** for icons. Material Symbols work like an icon font: you load the font once in your HTML, then display icons by writing the icon name inside a `<span>` element.

Google’s Material Symbols support different visual settings such as weight, fill, grade, and optical size, which can be controlled through CSS. 

### 1. Add the Google Fonts link

Add this inside the `<head>` of your HTML file:

```html
<link 
  href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&display=swap" 
  rel="stylesheet"
/>
````

Example:

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <link 
    href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&display=swap" 
    rel="stylesheet"
  />

  <link rel="stylesheet" href="./styles.css" />
  <title>My Project</title>
</head>
```

### 2. Add icons in your HTML

Use a `<span>` with the class `material-symbols-outlined`.

The text inside the span is the icon name.

```html
<span class="material-symbols-outlined" aria-hidden="true">north_east</span>
<span class="material-symbols-outlined" aria-hidden="true">water_drop</span>
<span class="material-symbols-outlined" aria-hidden="true">precision_manufacturing</span>
<span class="material-symbols-outlined" aria-hidden="true">compare_arrows</span>
<span class="material-symbols-outlined" aria-hidden="true">west</span>
<span class="material-symbols-outlined" aria-hidden="true">east</span>
```

For example, this:

```html
<span class="material-symbols-outlined" aria-hidden="true">east</span>
```

will display the `east` arrow icon.

### 3. Add the base CSS

Add this to your main CSS file:

```css
.material-symbols-outlined {
  font-family: 'Material Symbols Outlined';
  font-weight: normal;
  font-style: normal;
  font-size: 24px;
  line-height: 1;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  text-transform: none;
  letter-spacing: normal;
  white-space: nowrap;
  direction: ltr;

  font-variation-settings:
    'FILL' 0,
    'wght' 400,
    'GRAD' 0,
    'opsz' 24;
}
```

### 4. Custom icon styling

You can create your own icon utility classes.

```css
.feature-icon {
  width: 48px;
  height: 48px;
  border-radius: 999px;
  font-size: 26px;
}

.feature-icon--primary {
  color: #30e1db;
  background-color: rgba(48, 225, 219, 0.12);
}

.feature-icon--secondary {
  color: #e1a830;
  background-color: rgba(225, 168, 48, 0.12);
}
```

Example usage:

```html
<span 
  class="feature-icon feature-icon--primary material-symbols-outlined" 
  aria-hidden="true"
>
  water_drop
</span>

<span 
  class="feature-icon feature-icon--secondary material-symbols-outlined" 
  aria-hidden="true"
>
  precision_manufacturing
</span>
```

### 5. Filled icon example

To make an icon filled, change the `FILL` value from `0` to `1`.

```css
.icon-filled {
  font-variation-settings:
    'FILL' 1,
    'wght' 500,
    'GRAD' 0,
    'opsz' 24;
}
```

Usage:

```html
<span class="material-symbols-outlined icon-filled" aria-hidden="true">
  social_leaderboard
</span>
```

### 6. Accessibility note

If the icon is only decorative, use:

```html
aria-hidden="true"
```

Example:

```html
<span class="material-symbols-outlined" aria-hidden="true">east</span>
```

If the icon communicates important meaning, add visible text nearby or use an accessible label on the button/link.

Example:

```html
<button class="button">
  View more
  <span class="material-symbols-outlined" aria-hidden="true">north_east</span>
</button>
```

### 7. Icons used in this project

The project currently uses the following Material Symbols:

```html
north_east
water_drop
precision_manufacturing
compare_arrows
west
east
social_leaderboard
crossword
group
photo_camera
```

You can search for more icons in the Google Fonts Icons library.

```

Small note: Material Symbols are loaded as a font from Google Fonts, and the icon name inside the span acts like a “word” that gets replaced visually by the matching icon. Google’s official guide confirms this web setup and the variable settings like `FILL`, `wght`, `GRAD`, and `opsz`. :contentReference[oaicite:0]{index=0}
::contentReference[oaicite:1]{index=1}
```


<!-- Icons head link -->
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet">

<!-- icons -->
<span class="material-symbols-outlined" aria-hidden="true">north_east</span>
<span class="feature-icon feature-icon--primary material-symbols-outlined" aria-hidden="true">water_drop</span>
<span class="feature-icon feature-icon--secondary material-symbols-outlined" aria-hidden="true">precision_manufacturing</span>
<span class="feature-icon feature-icon--primary material-symbols-outlined" aria-hidden="true">compare_arrows</span>
<span class="material-symbols-outlined" aria-hidden="true">west</span>
<span class="material-symbols-outlined" aria-hidden="true">east</span>
<span class="material-symbols-outlined" aria-hidden="true">social_leaderboard</span>
<span class="material-symbols-outlined" aria-hidden="true">crossword</span>
<span class="material-symbols-outlined" aria-hidden="true">group</span>
<span class="material-symbols-outlined" aria-hidden="true">photo_camera</span>