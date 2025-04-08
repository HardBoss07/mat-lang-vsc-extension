# MAT Syntax

VS Code extension providing syntax highlighting and a custom color theme for the MAT programming language.

## Features

- Syntax highlighting for `.mat` files
- Custom color theme: **MAT-Lang Syntax Highlighting**
- Language configuration including comment support and bracket matching

## Usage
1. Open any `.mat` file - syntax highlighting will activate automatically.
2. To apply the custom theme:
   - Open Command Palette: `Ctrl+Shift+P`
   - Select: `Preferences: Color Theme`
   - Choose: **MAT-Lang Syntax Highlighting**

## Installation

### From VSIX

1. Build the `.vsix` package:
   ```bash
   vsce package
   ```
2. Install it in VS Code:
   ```bash
   code --install-extension mat-lang-syntax-0.0.1.vsix
   ```

## Contributing
Issues and PRs welcome in my [GitHub Repository](https://github.com/HardBoss07/mat-lang-vsc-extension)!