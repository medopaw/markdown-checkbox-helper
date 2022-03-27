# markdown-checkbox-helper README

VSCode extension.

1. Enables you to add Shortcuts to toggle states of a checkbox line in markdown files, including checked or not, strike-through or not, highlighted or not, etc.
2. Supports customization for more states and more shortcuts.

This is the keyboard shortcuts I added in my VSCode `keybindings.json`:

```json
{
    "key": "cmd+b",
    "when": "editorTextFocus && !editorReadonly",
    "command": "markdown-checkbox-helper.toggleStyleWrapping",
    "args": {
        "before": "**",
        "after": "**"
    }
},
{
    "key": "cmd+i",
    "when": "editorTextFocus && !editorReadonly",
    "command": "markdown-checkbox-helper.toggleStyleWrapping",
    "args": {
        "before": "*",
        "after": "*"
    }
},
{
    "key": "ctrl+=",
    "when": "editorTextFocus && !editorReadonly",
    "command": "markdown-checkbox-helper.toggleStyleWrapping",
    "args": {
        "before": "==",
        "after": "=="
    }
},
{
    "key": "ctrl+-",
    "when": "editorTextFocus && !editorReadonly",
    "command": "markdown-checkbox-helper.toggleStyleWrapping",
    "args": {
        "before": "~~",
        "after": "~~"
    }
},
```

Based on [Markdown All in One](https://github.com/yzhang-gh/vscode-markdown).
