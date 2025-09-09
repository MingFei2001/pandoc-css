# Pandoc CSS Theme Demo

This document demonstrates how various markdown elements are styled with the current theme.

## Typography and Headings

### This is a Level 3 Heading

#### This is a Level 4 Heading

##### This is a Level 5 Heading

###### This is a Level 6 Heading

Regular paragraph text with **bold text** and *italic text* and ***bold italic text***. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Code Examples

Here's some `inline code` within a paragraph. You can also have longer code blocks:

```python
def fibonacci(n):
    """Generate fibonacci sequence up to n terms."""
    a, b = 0, 1
    for _ in range(n):
        print(a, end=' ')
        a, b = b, a + b
    print()

fibonacci(10)
```

```javascript
// JavaScript example
function greetUser(name) {
    return `Hello, ${name}! Welcome to our site.`;
}

console.log(greetUser("World"));
```

```bash
# Shell commands
git clone https://github.com/user/repo.git
cd repo
npm install
npm run build
```

## Lists

### Unordered Lists
- First item in unordered list
- Second item with some longer text to show how wrapping works
- Third item
  - Nested item one
  - Nested item two
    - Double nested item
- Fourth item back at root level

### Ordered Lists
1. First ordered item
2. Second ordered item with **bold text**
3. Third ordered item
   1. Nested numbered item
   2. Another nested item
   3. Third nested item
4. Fourth item with `inline code`

### Task Lists
- [x] Completed task
- [x] Another completed task
- [ ] Incomplete task
- [ ] Another incomplete task

## Quotes and Citations

> This is a blockquote. Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
> Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

> **Note:** This is a blockquote with **bold text** and `inline code`.

## Links and References

Here are some [inline links](https://example.com) and [links with titles](https://github.com "GitHub Homepage").

You can also use reference-style links like [this one][ref1] or [this other one][ref2].

[ref1]: https://pandoc.org "Pandoc Official Site"
[ref2]: https://www.markdownguide.org "Markdown Guide"

## Tables

| Feature | Description | Status |
|---------|-------------|--------|
| **Syntax Highlighting** | Code blocks with language support | ✅ Complete |
| **Responsive Design** | Mobile-friendly layout | ✅ Complete |
| **Dark Mode** | Theme variants available | ✅ Complete |
| **Custom Fonts** | Typography customization | 🚧 In Progress |

| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Left text    | Center text    | Right text    |
| More left    | More center    | More right    |

## Horizontal Rules

Content before the rule.

---

Content after the rule.

## Mathematical Expressions

When using Pandoc with MathJax or similar:

Inline math: $E = mc^2$

Block math:
$$
\sum_{i=1}^{n} x_i = x_1 + x_2 + \cdots + x_n
$$

## Images

![Sample Image](https://via.placeholder.com/600x200/333333/FFFFFF?text=Sample+Image)

## Definition Lists

Term 1
:   Definition of term 1

Term 2
:   Definition of term 2 with more detailed explanation that might span
    multiple lines and include **formatting**.

## Footnotes

Here's a sentence with a footnote[^1]. And here's another one[^2].

[^1]: This is the first footnote.
[^2]: This is the second footnote with more details.

## Special Characters and Entities

- Em dash: —
- Ellipsis: …
- Copyright: ©
- Trademark: ™
- Arrows: → ← ↑ ↓
- Quotes: "Hello" 'World'

## Sample Code Documentation

### Function Reference

#### `processData(input, options)`

**Parameters:**
- `input` (string): The input data to process
- `options` (object): Configuration options
  - `format` (string): Output format ('json', 'xml', 'csv')
  - `validate` (boolean): Whether to validate input

**Returns:** Processed data in specified format

**Example:**
```javascript
const result = processData(myData, {
    format: 'json',
    validate: true
});
```

---

*This demo showcases the theme's styling for various markdown elements. Generated with ❤️ for the Pandoc CSS collection.*