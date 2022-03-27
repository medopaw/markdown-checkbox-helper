# markdown-checkbox-helper README

This is the README for your extension "markdown-checkbox-helper". After writing up a brief description, we recommend including the following sections.

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

## Features

Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something

## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension.

## Release Notes

Users appreciate release notes as you update your extension.

### 0.0.1

Initial release

-----------------------------------------------------------------------------------------------------------

## Following extension guidelines

Ensure that you've read through the extensions guidelines and follow the best practices for creating your extension.

* [Extension Guidelines](https://code.visualstudio.com/api/references/extension-guidelines)

## Working with Markdown

**Note:** You can author your README using Visual Studio Code.  Here are some useful editor keyboard shortcuts:

* Split the editor (`Cmd+\` on macOS or `Ctrl+\` on Windows and Linux)
* Toggle preview (`Shift+CMD+V` on macOS or `Shift+Ctrl+V` on Windows and Linux)
* Press `Ctrl+Space` (Windows, Linux) or `Cmd+Space` (macOS) to see a list of Markdown snippets

### For more information

* [Visual Studio Code's Markdown Support](http://code.visualstudio.com/docs/languages/markdown)
* [Markdown Syntax Reference](https://help.github.com/articles/markdown-basics/)

**Enjoy!**
