# VS Code Settings

## Font

- Operator Mono Lig

## Themes/Color

- [Just Black](https://marketplace.visualstudio.com/items?itemName=nur.just-black)
  - See [`editor.tokenColorCustomizations`](#settings) in my VS Code settings for a few modifications I make to the theme.
- [Github Light Theme](https://marketplace.visualstudio.com/items?itemName=Hyzeta.vscode-theme-github-light)
  - See [`editor.tokenColorCustomizations`](#settings) in my VS Code settings for a few modifications I make to the theme.

## Extensions

### Extension package names for easy install

```
xabikos.javascriptsnippets
christian-kohler.path-intellisense
jasonnutter.search-node-modules
infeng.vscode-react-typescript
jawandarajbir.react-vscode-extension-pack
fosshaas.fontsize-shortcuts
foxundermoon.shell-format
nur.just-black
digitalbrainstem.javascript-ejs-support
leizongmin.node-module-intellisense
dbaeumer.vscode-eslint
formulahendry.auto-close-tag
vunguyentuan.vscode-postcss
vscjava.vscode-java-dependency
xabikos.reactsnippets
mikestead.dotenv
orta.vscode-jest
pmneo.tsimporter
yoavbls.pretty-ts-errors
naumovs.color-highlight
mechatroner.rainbow-csv
bradlc.vscode-tailwindcss
christian-kohler.npm-intellisense
esbenp.prettier-vscode
visualstudioexptteam.intellicode-api-usage-examples
vscjava.vscode-java-debug
zignd.html-css-class-completion
sburg.vscode-javascript-booster
prisma.prisma
codeium.codeium
vscode-icons-team.vscode-icons
vscjava.vscode-java-pack
erikphansen.vscode-toggle-column-selection
quicktype.quicktype
dsznajder.es7-react-js-snippets
vscjava.vscode-java-test
ms-vscode.vscode-typescript-next
ritwickdey.liveserver
pranaygp.vscode-css-peek
wix.vscode-import-cost
vscjava.vscode-maven
ms-vscode.powershell
vscjava.vscode-gradle
visualstudioexptteam.vscodeintellicode
redhat.java
oracle.oracle-java
```

## Settings

```json
{
  // === Editor Core ===
  "editor.fontFamily": "Operator Mono Lig, JetBrains Mono, Fira Code, monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.lineHeight": 24,
  "editor.letterSpacing": 0.5,
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorBlinking": "solid",
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.detectIndentation": false,
  "editor.renderWhitespace": "boundary",
  "editor.renderFinalNewline": "on",
  "editor.trimAutoWhitespace": true,
  "editor.renderLineHighlight": "all",

  // === Suggestions & Productivity ===
  "editor.quickSuggestions": {
    "other": true,
    "comments": false,
    "strings": true
  },
  "editor.suggestSelection": "first",
  "editor.suggest.snippetsPreventQuickSuggestions": false,
  "editor.snippetSuggestions": "top",
  "editor.parameterHints.enabled": true,
  "editor.inlineSuggest.enabled": true,
  "editor.hover.enabled": true,

  // === Formatting & Code Style ===
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "editor.formatOnPaste": false,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "files.trimTrailingWhitespace": true,
  "files.insertFinalNewline": true,

  // === Visual Tweaks ===
  "editor.minimap.enabled": false,
  "editor.glyphMargin": false,
  "editor.scrollBeyondLastLine": false,
  "editor.smoothScrolling": false,
  "workbench.editor.showTabs": "none",
  "workbench.statusBar.visible": false,
  "workbench.sideBar.location": "right",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Just Black",
  "window.zoomLevel": 2,
  "editor.unicodeHighlight.invisibleCharacters": false,

  // === Token Customization ===
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": ["keyword.operator", "punctuation.separator"],
        "settings": {
          "fontStyle": ""
        }
      },
      {
        "scope": ["comment", "comment.block"],
        "settings": {
          "fontStyle": "italic",
          "foreground": "#7f7f7f"
        }
      },
      {
        "name": "envKeys",
        "scope": [
          "string.quoted.double.env",
          "source.env",
          "constant.numeric.env"
        ],
        "settings": {
          "foreground": "#3099e4"
        }
      }
    ]
  },

  // === Terminal ===
  "terminal.integrated.fontSize": 14,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.cursorBlinking": false,

  // === Git ===
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.openRepositoryInParentFolders": "never",

  // === Files ===
  "files.autoSave": "off",
  "files.exclude": {
    "**/.git": true,
    "**/.DS_Store": true,
    "**/node_modules": true,
    "**/dist": true
  },

  // === Search ===
  "search.exclude": {
    "**/node_modules": true,
    "**/bower_components": true,
    "**/*.code-search": true
  },
  "search.useIgnoreFiles": true,

  // === Screencast Mode===
  "screencastMode.keyboardOptions": {
    "showCommandGroups": false,
    "showCommands": false,
    "showKeybindings": true,
    "showKeys": false,
    "showSingleEditorCursorMoves": true
  },

  // === Telemetry / Privacy ===
  "telemetry.telemetryLevel": "off",
  "telemetry.feedback.enabled": false,

  // === ESLint / Prettier ===
  "eslint.enable": true,
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "vue",
    "html"
  ],

  // === Formatting by Language ===
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[scss]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[python]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[handlebars]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  // === Extensions / Explorer ===
  "extensions.ignoreRecommendations": true,
  "explorer.openEditors.visible": 9,
  "explorer.confirmDragAndDrop": false,
  "explorer.compactFolders": true,

  // === Database Clients ===
  "database-client.autoSync": true
}

```
