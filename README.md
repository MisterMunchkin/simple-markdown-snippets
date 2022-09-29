# Markdown Snippets for MDX and Docusaurus README

This is a VSCode extension snippet inspired by my laziness in not memorizing markdown symbols for Docusaurus with MDX.

## Features

Typing '!' in a .md/.mdx file gives you access to snippets like: !codeblock, !fmatter, !fmatter-sidebar, !admo, among [others](#list-of-snippets).

**Bold**, `Code` and *Italics* are also enabled to work with [Selected Text Keybinding](#keybindings-on-selected-text-support).

🔥**New**🔥 `!link` now works with selected text keybinding. The text you highlight will be enclosed inside the `[]`.

## Examples
![Screen Recording 2022-08-21 at 1 44 30 PM copy](https://user-images.githubusercontent.com/9417970/185778430-01e54351-a440-4462-8934-c2cb487b448b.gif)
![Screen Recording 2022-08-21 at 1 44 30 PM copy-2](https://user-images.githubusercontent.com/9417970/185778847-adf2e6a8-fe45-402d-b95b-8035bc9c5e85.gif)
![Screen Recording 2022-08-21 at 1 44 30 PM copy-3](https://user-images.githubusercontent.com/9417970/185778986-040c9555-a9c9-41db-a1d5-f5aa89f6f798.gif)

## List of Snippets
- **!codeblock**: codeblock with language option and title tab stops
- **!link**: made use of this snippet, It now works with selected text [keybinding](#keybindings-on-selected-text-support).
- **!fmatter**: snippet for the front matter with slug, title, authors, tags properties
- **!fmatter-sidebar**: snippet for the front matter with sidebar_label, and sidebar_position properties
- **!admo**: snippet for admonitions with type options
- **!export-component**: snippet for react export component with two prop options
- **!import-components**: snippet for react import component with name and path tabstops
- **!tab**: snippet for docusaurus-mdx tab with tabItem
- **!element**: snippet for React element
- **!bold**: snippet that works with selected text keybinding for **bold**
- **!italic**: snippet that works with selected text keybinding for *italic*
- **!code**: snippet that works with selected text keybinding for `code`

I also added a yaml.code-snippets so !authors would work
while editing in the front matter
- **!author**: author yaml code with name, title, url, image_url tabstops
- **!seo**: all SEO related front matter properties described here [Docusaurus SEO](https://docusaurus.io/docs/seo)

## Requirements

### MDX Support

This extension should work with .md files out of the box. For .mdx files, you would need to make file associations. To do that, simply click on the Plain Text at the bottom right of vs code and then '*Configure File Association for .mdx*'. Search for Markdown then you should be all set!

To make it easier for you, here's the relevant *settings.json* configuration:
```json title='settings.json'
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
### Keybindings on Selected Text Support
I also wanted **Bold**, `Code`, and *Italics* to work with selected text keybinding. So you can add this to your **keybindings.json** and update the keybinding to whatever you prefer.

```json title='keybindings.json'
{
    "key": "cmd+shift+b",
    "command": "editor.action.insertSnippet",
    "when": "editorTextFocus",
    "args": {
        "langId": "markdown",
        "name": "Markdown Bold Selected Text"
    }
},
{
    "key": "cmd+shift+c",
    "command": "editor.action.insertSnippet",
    "when": "editorTextFocus",
    "args": {
        "langId": "markdown",
        "name": "Markdown Code Selected Text"
    }
},
{
    "key": "cmd+shift+i",
    "command": "editor.action.insertSnippet",
    "when": "editorTextFocus",
    "args": {
        "langId": "markdown",
        "name": "Markdown Italic Selected Text"
    }
},
{
    "key": "cmd+shift+l",
    "command": "editor.action.insertSnippet",
    "when": "editorTextFocus",
    "args": {
        "langId": "markdown",
        "name": "Markdown Link Selected Text"
    }
}
```

## Installation

VS Code Market Place: [Markdown Snippets for MDX and Docusaurus](https://marketplace.visualstudio.com/items?itemName=MisterMunchkin.simple-markdown-snippets)

## Known Issues

There's no way to add keybindings directly onto the snippet extension. So you need to add the keybindings.json mentioned above to use the selected text keybindings.

**Current Supported Keybindings**
- **Bold**
- *Italic*
- `Code`
- [Link](#keybindings-on-selected-text-support)

## Contribution

Feel free to send a PR for any bugs or features you want to add to this.

## Release Notes

All version notes are now in CHANGELOG.md.

## Closing Thoughts

If you enjoy this VS Code extension, you can [buy me a ☕️](https://www.paypal.com/donate/?hosted_button_id=B9HDECYJ4CEF8). I also have a [blog site](https://blog.robindalmy.com) where I use this extension regularly and update it whenever I run into any issues or improvements I want to add while making blogs. 

**Enjoy!**
