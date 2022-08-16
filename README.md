# simple-markdown-snippets README

This is a vscode extension snippet inspired by my lazyness to not memorize markdown symbols for docusaurus with mdx.
I didn't add the usual markdown snippets on here because vs code already has that built in.

## Features

using the '!' gives you access to snippets like: !codeblock, !fmatter, !fmatter-sidebar, !admo, among others


### Examples
!fmatter and then !author

![tinywow_fmatter-with-author_4435317](https://user-images.githubusercontent.com/9417970/184831740-6c180455-72e2-4986-955c-1a9c5a83dd1e.gif)

!codeblock

![tinywow_codeblock_4435261](https://user-images.githubusercontent.com/9417970/184831874-3143b432-107c-4cec-b3e6-60969ed67a08.gif)

!admonition

![tinywow_admonition_4435162](https://user-images.githubusercontent.com/9417970/184831951-f9f67639-c31c-47c5-99a6-51b90447578d.gif)

!export-component

![tinywow_react-export-component_4435330](https://user-images.githubusercontent.com/9417970/184832206-c4e33074-f5fa-4856-91ae-48a39442fa48.gif)

## Requirements

This extension should work with .md files out of the box. For .mdx files, you would need to make file associations. To do that, simply click on the Plain Text at the bottom right of vs code and then 'Configure File Association for .mdx' then search for Markdown then you should be all set!

![tinywow_Screen Recording 2022-08-16 at 4 21 19 PM_4435553](https://user-images.githubusercontent.com/9417970/184833315-abc5479f-7643-4850-9e37-cd9408dcc326.gif)

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

## Known Issues

None so far.

## Contribution

Feel free to send a PR for any bugs or features you want to add on to this.

## Release Notes

Added snippets to main docusaurs, markdown, mdx code that isn't covered by vs codes built in markdown snippets.

### 1.0.0

Initial release of simple-markdown-snippets.

**Enjoy!**
