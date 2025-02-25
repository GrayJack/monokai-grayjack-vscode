# Change Log

All notable changes to the this extension will be documented in this file.

## 1.2.0
- UI: Define more `testing.` color configurations
- UI: Fix background color used in Inlay Hints
- UI: Fix highlight in search matches
- Feature: Add light Catppuccin theme (Latte) (First light theme!)
  - Done more for completion sake and as poc for future original light theme, as I never use light themes so white in the background. But if you like it, feel free to check it out as well

## 1.1.0
- UI: Fix unnecessary code opacity configuration
- UI: Fix output background color
- UI: Fix coloring of native git graph label foreground
- UI: Add detail border between activity bar and panel
    - Could happen when panel is configured as left or right aligned or when sidePanel is not active
- Feature: Add dark Catppuccin themes (Frappé, Macchiato and Mocha)

## 1.0.0
- **Breaking Change:** Rework all themes from the ground up
  - Solved inconsistencies between themes
  - Support almost entire UI theme options as VSCode 1.97 (A few todos left for entire)
- **Breaking Change:** Rename themes and deprecate as legacy
  - These themes will continue to be updated for TextMate and Semantic Highlight changes, but UI coloring will no longer be worked on. More information on this can be found on the README file.
- Add a new `Monokai` variant: "GrayJack's Monokai (Lunarized)"
  - Name given by my partner, based on the background color reminding her of the moon. The name worked so well since it already have a solarized version
- Perf: Reduce package size by not packing useless files for the theme to work
- Move preview images to folder

## 0.15.2
- Tweak Semantic Highlight for Rust ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer)): Handle unsafe attribute specially
- Tweak Semantic Highlight for Rust ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer)): Handle const and static custom tokens specially

## 0.15.1
-   UI: Fix issue with diff editor hiding lighter texts on some themes (Also tweak a bit the color for the ones that didn't had the issue)

## 0.15.0
-   UI: Nord: Fix shadows being invisible on some of the backgrounds
-   UI: Monokai and Monokai Pastel: Make list dropdown background slightly darker
-   UI: Monokai Solarized: Change color of the active line
-   UI: One Dark: Reduce contrast of the "orange" color
-   UI: Ariake and Monokai Solarized: Fix selection color on menus and inputs
-   Tweak TextMate for TS/JS -> Tweak property highlight for JS/TS
-   Tweak TextMate for Rust -> Add scope used by recent version of the TextMate grammar
-   Tweak semantic highlight for [Rust]((https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer)) -> Rework the highlight for rust attributes
    - This change makes derives names being italic like all interfaces but remain the color of attributes
    - This also makes custom codes inside attributes remain colorized as code instead of overwriting with the attribute color.
    - This also makes literals inside attributes remain colorized their literal color instead of overwriting with the attribute color.
-   Add initial support for Koka
-   Fix JSON warnings

## 0.14.0

-   UI: Improve stick scroll visibility
-   Tweak semantic highlight for [Swift](https://marketplace.visualstudio.com/items?itemName=sswg.swift-lang) -> handle attributes (they have the `modifier` token for some reason)
-   Tweak TextMate for [Swift](https://marketplace.visualstudio.com/items?itemName=sswg.swift-lang) -> handle enum variant
-   Tweak semantic highlight for [Java](https://marketplace.visualstudio.com/items?itemName=redhat.java) -> handle `@` annotations
-   Tweak semantic highlight for [Java](https://marketplace.visualstudio.com/items?itemName=redhat.java) -> colorize `readonly` as constant color
-   Tweak semantic and TextMate highlight for [Zig](https://marketplace.visualstudio.com/items?itemName=ziglang.vscode-zig) -> namespace is now faded color of the normal text color

## 0.13.0

-   Make Punctuation a faded color of the normal text color.
    -   Provides a better contrast between both without removing the information or making it too distracting.
-   Ariake, Monokai (Solarized) and OneDark themes have a slightly lighter text color.
    -   Improves contrast between the text and the background.
-   Unify the color of the namespace token.
    -   Uses a slightly faded color of the normal text color.
-   Tweak semantic highlight for Python ([Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance))
    -   Color global read-only variables as constant.
-   Tweak TextMate colors for Python
    -   Format placeholder is styled like format placeholder in semantic highlight.

## 0.12.7

-   Improvements to selected text background for Ariake, Monokai (Solarized), One Dark

## 0.12.6

-   Tweak TextMate colors for ARM assembly ([Arm Assembly](https://marketplace.visualstudio.com/items?itemName=dan-c-underwood.arm))
-   Tweak TextMate colors for ARM64 assembly ([ARM64 Assembly](https://marketplace.visualstudio.com/items?itemName=MKornelsen.vscode-arm64))

## 0.12.5

-   Tweak semantic highlight for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Tweak TextMate colors for Racket
    ([Magic Racket](https://marketplace.visualstudio.com/items?itemName=evzen-wybitul.magic-racket))

## 0.12.4

-   Tweak semantic highlight for C++
    ([C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools))
-   Tweak TextMate colors for Swift

## 0.12.3

-   Tweak semantic highlight for Lua
    ([Lua](https://marketplace.visualstudio.com/items?itemName=sumneko.lua))

## 0.12.2

-   Tweak TextMate colors for Zig
    ([Zig](https://marketplace.visualstudio.com/items?itemName=tiehuis.zig))

## 0.12.1

-   Tweak TextMate colors for Python
-   Fix a mistake on TextMate

## 0.12.0

-   Tweak semantic highlight for JavaScript (Build-in and
    [Deno](https://marketplace.visualstudio.com/items?itemName=denoland.vscode-deno))
-   Tweak semantic highlight for TypeScript (Build-in and
    [Deno](https://marketplace.visualstudio.com/items?itemName=denoland.vscode-deno))
-   Tweak semantic highlight for Kotlin
    ([Kotlin](https://marketplace.visualstudio.com/items?itemName=fwcd.kotlin))
-   Simplify coloring of `member` token
-   Simplify coloring of `namespace` token (there is more languages the uses `.`
    (dot) to access namespace as well as fields and methods access than languages
    that uses a different token to namespaces like Rust and C++)

## 0.11.0

-   Add coloring for Inlay Hints
-   Add coloring for Rust-Analyzer Inlay Hints
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Tweak UI colors for Nord and Tokyo Night themes
-   Tweak semantic highlight for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Add semantic coloring for `record` tokens
-   Tweak semantic highlight for Java
    ([Language Support for Java(TM) by Red Hat](https://marketplace.visualstudio.com/items?itemName=redhat.java))

## 0.10.1

-   Tweak semantic highlight for overloaded operator C#
    ([C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp))
-   Tweak semantic highlight for overload operator in C++
    ([C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools))

## 0.10.0

-   Add new theme: Nord GrayJack
-   Tweak colors on Ariake, Tokyo Night, OneDark

## 0.9.2

-   Change colors of line numbers on Ariake, Monokai (Solarized), One Dark and
    Tokyo Night
    -   Improvements to colors when on diff view
    -   Makes more colorful

## 0.9.1

-   Fix diff colors on Tokyo Night GrayJack
-   Fix peek view for Tokyo Night GrayJack
-   Change diff colors for Ariake GrayJack

## 0.9.0

-   Tweak UI for Monokai (Solarized), Ariake and OneDark
-   Add new theme: Tokyo Night GrayJack

## 0.8.4

-   Tweak TextMate colors for C++
    ([Better C++ Syntax](https://marketplace.visualstudio.com/items?itemName=jeff-hykin.better-cpp-syntax))
-   Tweak TextMate color for C#
    ([C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp))

## 0.8.3

-   Tweak semantic highlight for C++
    ([C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools))
-   Tweak semantic highlight for C#
    ([C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp))
-   Tweak TextMate for C#
    ([C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp))
-   Tweak TextMate colors for Rust files (Build-in)

## 0.8.2

-   Fix missing TextMate for AGDA
    ([language-agda](https://marketplace.visualstudio.com/items?itemName=j-mueller.agda))

## 0.8.1

-   Add support for bracket colorization for all themes
-   Tweak TextMate for F#
    ([Ionide-fsharp](https://marketplace.visualstudio.com/items?itemName=Ionide.Ionide-fsharp))
-   Tweak TextMate for AGDA
    ([language-agda](https://marketplace.visualstudio.com/items?itemName=j-mueller.agda))

## 0.8.0

-   Change some Ariake colors
-   Change some OneDark colors
-   Tweak button colors on Ariake GrayJack, Monokai GrayJack (Solarized) and
    OneDark GrayJack
-   Tweak semantic styling on error variant in Zig
    ([ZLS for VSCode](https://marketplace.visualstudio.com/items?itemName=AugusteRame.zls-vscode))

## 0.7.0

-   Add theme Ariake GrayJack
-   Fix: textMate tokens only accepts `fontStyle`
-   Tweak sidebar colors on Monokai GrayJack and Monokai GrayJack (Pastel)
-   Tweak ignored resources files color on Monokai GrayJack (Solarized) and
    OneDark GrayJack

## 0.6.3

-   Tweak TextMate colors for dune files
    ([Ocaml Platform](https://marketplace.visualstudio.com/items?itemName=ocamllabs.ocaml-platform))
-   Tweak sidebar colors on Monokai GrayJack and Monokai GrayJack (Pastel)

## 0.6.2

-   Fix small mistake on UI colors

## 0.6.1

-   Fix small mistake on UI colors

## 0.6.0

-   Add theme OneDark GrayJack
-   Tweak UI colors on Monokai GrayJack (Solarized)
-   Tweak semantic highlight so when generic font stylization don't lose inherited
    stylization
-   Tweak semantic highlight for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer)):
    unsafe callables are now italic to distinct from mutable callables.

## 0.5.0

-   Add theme Monokai GrayJack (Solarized)
-   Tweak UI colors

## 0.4.0

-   Tweak TextMate for Racket
    ([Magic Racket](https://marketplace.visualstudio.com/items?itemName=evzen-wybitul.magic-racket))
-   Tweak UI colors
-   Tweak standard semantic tokens for types (Concrete Types aren't italic,
    Interfaces remain italic)

## 0.3.8

-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Tweak semantic tokens coloring for TypeScript (Native plugin/JavaScript and
    TypeScript next)
-   Tweak TextMate for TypeScript (Build-in)
-   Tweak TextMate for C++
    ([Better C++ Syntax](https://marketplace.visualstudio.com/items?itemName=jeff-hykin.better-cpp-syntax))

## 0.3.7

-   Fix CHANGELOG

## 0.3.6

-   Tweak semantic tokens coloring for TOML
    ([Even Better TOML](https://marketplace.visualstudio.com/items?itemName=tamasfe.even-better-toml))
-   Tweak TextMate for TOML
    ([Even Better TOML](https://marketplace.visualstudio.com/items?itemName=tamasfe.even-better-toml))

## 0.3.5

-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))

## 0.3.4

-   Tweak semantic tokens coloring for Zig
    ([ZLS for VSCode](https://marketplace.visualstudio.com/items?itemName=AugusteRame.zls-vscode))
-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Tweak semantic tokens coloring for Go
    ([Go with gopls](https://marketplace.visualstudio.com/items?itemName=golang.Go))

## 0.3.3

-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))

## 0.3.2

-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))

## 0.3.1

-   Fix CHANGELOG and README in the marketplace

## 0.3.0

-   Change bits of overall theme
-   Tweaks semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))

## 0.2.11

-   Tweaks on TextMate for Rust (build-in plugin)
-   Tweaks on TextMate for Python (Build-in plugin)
-   Tweaks on TextMate for HTML (Build-in plugin)
-   Tweaks on TextMate for CSS-like (Build-in plugin)
-   Tweaks on TextMate for Nim
    ([Nim](https://marketplace.visualstudio.com/items?itemName=kosz78.nim)/[Nim Alt](https://marketplace.visualstudio.com/items?itemName=garym.nim-alt))
-   Tweaks on TextMate for D-lang
    ([Dlang](https://marketplace.visualstudio.com/items?itemName=webfreak.code-d))
-   Tweak semantic tokens coloring for Rust
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))
-   Tweak semantic tokens coloring for Python
    ([Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance))
-   Tweak semantic tokens coloring for Zig
    ([ZLS for VSCode](https://marketplace.visualstudio.com/items?itemName=AugusteRame.zls-vscode))

## 0.2.10

-   Fix semantic tokens with callable modifier not being properly colorized

## 0.2.9

-   Add color for semantic tokens with Rust callable modifier
    ([rust-analyzer](https://marketplace.visualstudio.com/items?itemName=matklad.rust-analyzer))

## 0.2.8

-   Tweaks on TextMate for Janet, Python, D and Nim
-   More tweaks on TextMate for C/C++

## 0.2.7

-   Tweaks on TextMate for C/C++

## 0.2.6

-   Tweaks on TextMate for Kotlin and Go

## 0.2.5

-   Tweaks on semantic highlight for TypeScript and Java
    ([Language Support for Java](https://marketplace.visualstudio.com/items?itemName=redhat.java))
-   Small tweak on TextMate

## 0.2.4

-   Tweaks on several text-mate grammar colors

## 0.2.3

-   Change the Brown colors in the Pastel variant

## 0.2.2

-   Add a hover colors different of the active window

## 0.2.1

-   Fix a color not matching the color theme in settings

## 0.2.0

-   Change gray colors
-   Add many more color customization (menu, lens, tree-view, etc)
-   Add a pastel variant of the theme

## 0.1.0

-   Initial release
