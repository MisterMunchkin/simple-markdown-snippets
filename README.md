# simple-markdown-snippets README

This is a vscode extension snippet inspired by my lazyness to not memorize markdown symbols for docusaurus with mdx.
I didn't add the usual markdown snippets on here because vs code already has that built in.

## Features

using the '!' gives you access to snippets like: !codeblock, !fmatter, !fmatter-sidebar, !admo, among others!

NOTE: ADD ANIMATIONS HERE

Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

This extension should work with .md files out of the box. For .mdx files, you would need to make file associations. To do that, simply click on the Plain Text at the bottom right of vs code and then 'Configure File Association for .mdx' then search for Markdown then you should be all set!

To make it easier for you, here's the relevant settings.json configuration:
```
    "editor.quickSuggestions": {
        "comments": "inline",
        "strings": "inline"
    },
    "[markdown]": {
        "editor.quickSuggestions": {
            "other": "on",
            "comments": "inline",
            "strings": "inline"
        }
    },
    "files.associations": {
        "*.mdx": "markdown"
    }
```

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: Enable/disable this extension.
* `myExtension.thing`: Set to `blah` to do something.

## Known Issues

Calling out known issues can help limit users opening duplicate issues against your extension.

## Contribution

Feel free to send a PR for any bugs or features you want to add on to this.

## Release Notes

Added snippets to main docusaurs, markdown, mdx code that isn't covered by vs codes built in markdown snippets.

### 1.0.0

Initial release of simple-markdown-snippets.

**Enjoy!**
