# Change Log

All notable changes to the "mat-lang-syntax" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.0.2] - 2026-09-25

### Added

- **Language Keywords**: Full syntax highlighting for `fori`, `loop`, `match`, `import`, `pub`, `struct`, `enum`, `fn`, `let`, `mut`, `return`, `if`, `else`, `while`, `for`, `in`, `break`, and `continue`[cite: 1].
- **Boolean Literals**: Recognized `tru` and `fal` primitives[cite: 1, 3].
- **Built-in Types & ADTs**: Primitive types (`int`, `i32`, `i16`, `i8`, `f64`, `bool`, `char`) and standard library types (`Result`, `Ok`, `Err`, `Vec`, `String`)[cite: 1, 3].
- **Literals & Separators**: Support for hexadecimal (`0xA5`), binary (`0b10100100`), floating-point values, and underscore digit separators (`1_000_000`)[cite: 1, 3].
- **String Interpolation**: Embedded expression highlighting inside double-quoted strings (`"{var}"`)[cite: 1, 3].
- **Operators**: Unary mutation (`++`, `--`), bitwise shift compounds (`<<=`, `>>=`), namespace resolution (`::`), and match arm arrows (`=>`, `->`)[cite: 1, 3].
- **Auto-Indentation**: Configured automatic brace, bracket, and pattern matching indentation rules[cite: 1, 6].

### Changed

- Updated publisher handle to `HardBoss07`[cite: 4].
- Aligned theme scope selectors from `.matlang` to `.mat` so custom colors apply cleanly to `.mat` files[cite: 5, 7].

### Fixed

- Fixed duplicate `https://` prefix in `package.json` repository URL[cite: 4].

## [0.0.1]

- Initial pre-release of MAT language syntax extension.
