# MAT Syntax Highlighting

Official VS Code extension providing syntax highlighting, auto-indentation, and a custom color theme for the **mat** programming language (`.mat`).

---

## Features

- **Full Keyword & Syntax Coverage**: Highlighting for control flow (`fori`, `for`, `in`, `while`, `loop`, `match`, `if`, `else`, `return`, `break`, `continue`), visibility (`pub`), imports (`import`), and declaration keywords (`fn`, `let`, `mut`, `struct`, `enum`).
- **Boolean Primitives**: Highlights `mat` native booleans (`tru` and `fal`).
- **Rich Number Formats**: Full support for decimal, hexadecimal (`0xA5`), binary (`0b10100100`), floating-point values, and underscore digit separators (`1_000_000`).
- **String Interpolation**: Distinct inline highlighting for expressions embedded inside string literals (`"Hello {name}"`).
- **Operators & Mutations**: Full tokenizer coverage for unary mutations (`++`, `--`), compound bitwise shift operators (`<<=`, `>>=`), namespace resolution (`::`), match arrows (`=>`), and type signatures (`->`).
- **Type Highlighting**: Support for primitive types (`int`, `i32`, `i16`, `i8`, `f64`, `bool`, `char`) and standard built-ins (`Result`, `Ok`, `Err`, `Vec`, `String`).
- **Custom Color Theme**: Includes the tuned **MAT-Lang Syntax Highlighting** dark color theme.
- **Language Integration**: Auto-closing pairs, comment toggling (`//`), bracket matching, and automatic brace/pattern-match indentation.

---

## Code Showcase (`example.mat`)

```mat
import std::io;

pub struct Point {
    pub x: int,
    pub y: int,
}

pub enum Shape {
    Circle(f64),
    Rectangle(Point, Point),
}

fn main() {
    let mut score: int = 50;
    let is_active: bool = tru;
    let mask: i32 = 0xA5;

    // String Interpolation
    let name: String = "World";
    println("Hello {name}!");

    // Operators & Loops
    score++;
    score <<= 2;

    fori (let i: int = 0; i < 5; i++) {
        score += i;
    }

    // Pattern Matching
    let shape: Shape = Shape::Circle(3.14);
    match shape {
        Shape::Circle(r) => println("Radius: {r}"),
        Shape::Rectangle(p1, p2) => println("Rectangle"),
    }
}
```

---

## Usage

1. Open any `.mat` file—syntax highlighting will activate automatically.
2. To enable the optional bundled color theme:

- Open the Command Palette: `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS)
- Select: **`Preferences: Color Theme`**
- Choose: **`MAT-Lang Syntax Highlighting`**

---

## Installation

### From VS Code Marketplace

Search for `MAT Syntax` in the VS Code Extensions tab (`Ctrl+Shift+X`), or install directly via CLI:

```bash
code --install-extension m4tt3o.mat-lang-syntax
```

### From Local VSIX Package

1. Build the VSIX package from the extension directory:

```bash
vsce package
```

2. Install the generated `.vsix` package:

```bash
code --install-extension mat-lang-syntax-0.0.2.vsix
```

---

## Contributing

Issues, feedback, and pull requests are welcome on [GitHub](https://github.com/HardBoss07/mat-lang-vsc-extension)!
