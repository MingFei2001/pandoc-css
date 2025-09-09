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
pandoc -s input.md -o output.html --css=pandoc-css/themes/basic/dark.css

# Convert to PDF
pandoc input.md -o output.pdf --css=pandoc-css/themes/basic/dark.css --pdf-engine=wkhtmltopdf
```

## Try It Out

Test any theme using the included demo file:

```bash
# Test with the Nord theme
pandoc -s demo.md -o demo-nord.html --css=themes/editor-inspired/nord.css

# Test with Catppuccin Mocha
pandoc -s demo.md -o demo-mocha.html --css=themes/catppuccin/catppuccin-mocha.css

# Test with your own document
pandoc document.md -o document.html --css=themes/basic/light.css
```

The `demo.md` file includes various markdown elements (headings, code blocks, tables, lists, etc.) so you can see how each theme handles different content types.

## Available Themes

### Basic Themes
- `themes/basic/light.css` - Clean light theme
- `themes/basic/dark.css` - Modern dark theme

### Editor-Inspired Themes
- `themes/editor-inspired/nord.css` - Arctic-inspired Nord theme
- `themes/editor-inspired/onedark.css` - Atom's One Dark theme
- `themes/editor-inspired/everforest.css` - Green forest theme
- `themes/editor-inspired/kanagawa.css` - Japanese-inspired theme
- `themes/editor-inspired/monokai.css` - Classic Monokai theme
- `themes/editor-inspired/tokyo-night.css` - Tokyo Night theme

### Gruvbox Collection
- `themes/gruvbox/gruvbox-light.css` - Gruvbox light variant
- `themes/gruvbox/gruvbox-dark.css` - Gruvbox dark variant

### Solarized Collection
- `themes/solarized/solarized-light.css` - Solarized light theme
- `themes/solarized/solarized-dark.css` - Solarized dark theme

### Catppuccin Collection
- `themes/catppuccin/catppuccin-latte.css` - Light, warm pastel theme
- `themes/catppuccin/catppuccin-frappe.css` - Cool, muted theme
- `themes/catppuccin/catppuccin-macchiato.css` - Rich, darker theme
- `themes/catppuccin/catppuccin-mocha.css` - Deep dark theme

## Customization

You can customize fonts by adding your own CSS after the theme. For example, to use JetBrains Mono Nerd Font:

```css
body {
  font-family: "JetBrains Mono", monospace;
}

pre, code {
  font-family: "JetBrains Mono Nerd Font", monospace;
}
```

Save this as `custom.css` and use both files:
```bash
pandoc -s input.md -o output.html --css=pandoc-css/themes/basic/dark.css --css=custom.css
```

## Acknowledgments

- [Pandoc](https://pandoc.org/) - Universal document converter
- [Nord](https://www.nordtheme.com/) - Arctic-inspired color palette
- [Catppuccin](https://github.com/catppuccin/catppuccin) - Soothing pastel theme
- [One Dark](https://github.com/atom/atom/tree/master/packages/one-dark-syntax) - Atom's syntax theme
- [Gruvbox](https://github.com/morhetz/gruvbox) - Retro groove color scheme
- [Solarized](https://ethanschoonover.com/solarized/) - Precision colors for machines and people
- [Everforest](https://github.com/sainnhe/everforest) - Green based color scheme
- [Kanagawa](https://github.com/rebelot/kanagawa.nvim) - NeoVim dark colorscheme inspired by Katsushika Hokusai
- [Monokai](https://monokai.pro/) - Original color scheme by Wimer Hazenberg
- [Tokyo Night](https://github.com/enkia/tokyo-night-vscode-theme) - Clean dark theme

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author Comment

*I totally vibe coded this project lol.*
