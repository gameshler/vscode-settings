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
  "diffEditor.ignoreTrimWhitespace": false,
  "editor.detectIndentation": true,
  "editor.fontFamily": "Operator Mono Lig",
  "editor.fontLigatures": true,
  "editor.fontSize": 13,
  "editor.formatOnPaste": false,
  "editor.inlineSuggest.enabled": true,
  "editor.lineHeight": 0,
  "editor.linkedEditing": true,
  "editor.minimap.enabled": false,
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.snippetSuggestions": "top",
  "editor.suggestSelection": "first",
  "editor.tabSize": 2,
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
          "foreground": "#F5F"
        }
      },
      {
        "name": "envKeys",
        "scope": "string.quoted.double.env,source.env,constant.numeric.env",
        "settings": {
          "foreground": "#3099e4"
        }
      }
    ]
  },
  "editor.unicodeHighlight.invisibleCharacters": false,
  "emmet.showAbbreviationSuggestions": false,
  "eslint.enable": true,
  "eslint.validate": ["vue", "react", "typescript", "html", "javascript"],
  "explorer.openEditors.visible": 1,
  "extensions.ignoreRecommendations": true,
  "git.autofetch": true,
  "git.openRepositoryInParentFolders": "never",
  "markdown.preview.fontSize": 36,
  "screencastMode.keyboardOptions": {
    "showCommandGroups": false,
    "showCommands": false,
    "showKeybindings": true,
    "showKeys": false,
    "showSingleEditorCursorMoves": true
  },
  "search.exclude": {
    "**/*.code-search": true,
    "**/bower_components": true,
    "**/node_modules": true
  },
  "search.useIgnoreFiles": false,

  "terminal.integrated.fontSize": 14,

  "window.zoomLevel": 4,
  "workbench.colorTheme": "Github Light Theme",
  "workbench.editor.labelFormat": "medium",
  "workbench.editor.showTabs": "none",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.sideBar.location": "right",
  "workbench.startupEditor": "newUntitledFile",
  "workbench.statusBar.visible": false,
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[handlebars]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
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
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[scss]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[python]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
  "telemetry.feedback.enabled": false,
  "database-client.autoSync": true,
  "explorer.confirmDragAndDrop": false,
  "explorer.compactFolders": false
}
```
