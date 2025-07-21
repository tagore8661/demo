# HTML Document Structure

## Basic HTML Document Structure

Every HTML document follows a standard structure. Here's the basic template:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

## Explanation of Each Component

### 1. DOCTYPE Declaration
```html
<!DOCTYPE html>
```
- **Purpose**: Tells the browser which version of HTML to use
- **HTML5**: Uses the simple `<!DOCTYPE html>`
- **Must be**: The very first line in your HTML document
- **Case insensitive**: Can be written in uppercase or lowercase

### 2. HTML Root Element
```html
<html lang="en">
```
- **Purpose**: The root element that contains all other elements
- **lang attribute**: Specifies the language of the document
- **Accessibility**: Helps screen readers and search engines
- **Common values**: "en" (English), "es" (Spanish), "fr" (French)

### 3. Head Section
```html
<head>
    <!-- Metadata goes here -->
</head>
```
- **Purpose**: Contains metadata about the document
- **Not visible**: Content here doesn't appear on the webpage
- **Contains**: Title, meta tags, links to stylesheets, scripts

#### Common Head Elements:

**Meta Charset**
```html
<meta charset="UTF-8">
```
- Specifies character encoding
- UTF-8 supports all languages and special characters

**Viewport Meta Tag**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- Controls how the page is displayed on mobile devices
- Essential for responsive design

**Title Element**
```html
<title>Document Title</title>
```
- Appears in browser tab
- Used by search engines
- Important for SEO

**Other Common Meta Tags**
```html
<meta name="description" content="Page description">
<meta name="keywords" content="keyword1, keyword2">
<meta name="author" content="Author Name">
```

### 4. Body Section
```html
<body>
    <!-- Visible content goes here -->
</body>
```
- **Purpose**: Contains all visible content of the webpage
- **Everything visible**: Text, images, videos, forms, etc.
- **Structure**: Where you build your page layout

## HTML Element Anatomy

### Basic Element Structure:
```html
<tagname attribute="value">Content</tagname>
```

**Components:**
1. **Opening Tag**: `<tagname>`
2. **Attributes**: `attribute="value"`
3. **Content**: Text or other elements
4. **Closing Tag**: `</tagname>`

### Self-Closing Elements:
```html
<img src="image.jpg" alt="Description">
<br>
<hr>
<input type="text">
```

## Nesting and Hierarchy

HTML elements can be nested inside other elements:

```html
<div>
    <h1>Main Heading</h1>
    <p>This is a paragraph with <strong>bold text</strong> inside.</p>
    <ul>
        <li>First item</li>
        <li>Second item</li>
    </ul>
</div>
```

**Rules for Nesting:**
- Elements must be properly closed
- Inner elements must close before outer elements
- Maintain proper indentation for readability

## Comments in HTML

```html
<!-- This is a comment -->
<!-- 
    This is a 
    multi-line comment 
-->
```

**Uses:**
- Document your code
- Temporarily disable code
- Leave notes for other developers
- Not visible to users

## Best Practices

1. **Always include DOCTYPE**: Ensures consistent rendering
2. **Use semantic HTML**: Choose elements based on meaning
3. **Proper indentation**: Makes code readable
4. **Close all tags**: Prevents rendering issues
5. **Use lowercase**: For tag names and attributes
6. **Quote attributes**: Always use quotes around attribute values
7. **Validate your HTML**: Use W3C validator to check for errors