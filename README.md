# Pandoc CSS

A collection of CSS themes for styling HTML documents generated with [Pandoc](https://pandoc.org/), a universal document converter that can convert between many different markup formats.

## Usage

1. Clone this repository:
```bash
git clone https://github.com/MingFei2001/pandoc-css.git
```

2. Use it with Pandoc's `--css` option to convert Markdown to styled HTML or PDF:

```bash
# Convert to HTML
pandoc -s input.md -o output.html --css=pandoc-css/dark.css

# Convert to PDF
pandoc input.md -o output.pdf --css=pandoc-css/dark.css --pdf-engine=wkhtmltopdf
```

Example:
```bash
pandoc document.md -o document.html --css=pandoc-css/light.css
```

## Available Themes

- `light.css` - Light theme
- `dark.css` - Dark theme
- `nord.css` - Nord theme
- `onedark.css` - OneDark theme
- `catppuccin/` - Catppuccin theme variants

## Acknowledgments

- [Pandoc](https://pandoc.org/) - Universal document converter
- [Nord](https://www.nordtheme.com/) - Arctic-inspired color palette
- [Catppuccin](https://github.com/catppuccin/catppuccin) - Soothing pastel theme
- [One Dark](https://github.com/atom/atom/tree/master/packages/one-dark-syntax) - Atom's syntax theme

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
