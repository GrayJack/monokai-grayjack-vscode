# GrayJack Themes

My collection of themes based on classic/famous themes.

For now only themes based on Ariake, Monokai, Nord, OneDark and Tokyo Night

## Monokai GrayJack

![Preview Monokai Grayjack 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-monokai.png)

![Preview Monokai Grayjack 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-monokai.png)

## Monokai GrayJack (Pastel)

![Preview Monokai Grayjack (Pastel) 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-monokaipastel.png)

![Preview Monokai Grayjack (Pastel) 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-monokaipastel.png)

## Monokai GrayJack (Solarized)

![Preview Monokai Grayjack (Solarized) 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-monokaisolarized.png)

![Preview Monokai Grayjack (Solarized) 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-monokaisolarized.png)

## OneDark GrayJack

![Preview OneDark Grayjack 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-onedark.png)

![Preview OneDark Grayjack 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-onedark.png)

## Ariake GrayJack

![Preview Ariake Grayjack 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-ariake.png)

![Preview Ariake Grayjack 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-ariake.png)

## Tokyo Night GrayJack

![Preview Tokyo Night Grayjack 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-tokyonight.png)

![Preview Tokyo Night Grayjack 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-tokyonight.png)

## Nord GrayJack

![Preview Nord Night Grayjack 1](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-welcome-nord.png)

![Preview Nord Night Grayjack 2](https://raw.githubusercontent.com/GrayJack/monokai-grayjack-vscode/master/preview-code-nord.png)

## Customization

Didn't like something the way I did? You can easily change the configuration in
your JSON configuration file

### Workbench example

```jsonc
"workbench.colorCustomizations": {
    "[Monokai GrayJack]": {
        "sideBar.background": "#347890"
    },
    "[Monokai GrayJack (Pastel)]": {
        "sideBar.background": "#347890"
    }
}
```

You can find a list of all thing you can change in the workbench
[here](https://code.visualstudio.com/api/references/theme-color)

### TextMate Scope Color and Styling

```jsonc
"editor.tokenColorCustomizations": {
    // simple example
    "[Monokai GrayJack]": {
        "comments": "#229977"
    },

    "[Monokai GrayJack (Pastel)]": {
        "textMateRules": [
            {
                "scope": "support.type.property-name.json",
                "settings": {
                    "foreground": "#229977",
                    "fontStyle": "italic"
                }
            }
        ]
    }
},
```

### Semantic Tokens Color and Styling

```jsonc
"editor.semanticTokenColorCustomizations": {
    "[Monokai Grayjack]": {
        "enabled": true,
        "rules": {
            "comment": {
                "foreground": "#229977",
                "bold": true
            },
            // For a specific language
            "comment:java": {
                "foreground": "#229977",
                "bold": false
            }
        }
    }
},
```

The rules follow the pattern: `<token>[.<modifier>][:<language-id>]` where what
is between angle bracket is mandatory and what is between square brackets are
optional

You can find the Semantic Tokens and for TextMate Scope of a part of your code
with the VS Code command `Developer: Inspect Editor Tokens and Scopes`.

For more about theme customization:
https://code.visualstudio.com/docs/getstarted/themes

More on TextMate Scopes Highlight:
https://code.visualstudio.com/api/extension-guides/color-theme

More on Semantic Highlight:
https://code.visualstudio.com/api/language-extensions/semantic-highlight-guide
