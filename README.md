# Markdown Snippets for MDX and Docusaurus README

This is a vscode extension snippet inspired by my lazyness to not memorize markdown symbols for docusaurus with mdx.
I didn't add the usual markdown snippets on here because vs code already has that built in.

## Features

using the '!' gives you access to snippets like: !codeblock, !fmatter, !fmatter-sidebar, !admo, among others

## Examples
![Screen Recording 2022-08-21 at 1 44 30 PM copy](https://user-images.githubusercontent.com/9417970/185778430-01e54351-a440-4462-8934-c2cb487b448b.gif)
![Screen Recording 2022-08-21 at 1 44 30 PM copy-2](https://user-images.githubusercontent.com/9417970/185778847-adf2e6a8-fe45-402d-b95b-8035bc9c5e85.gif)
![Screen Recording 2022-08-21 at 1 44 30 PM copy-3](https://user-images.githubusercontent.com/9417970/185778986-040c9555-a9c9-41db-a1d5-f5aa89f6f798.gif)

## List of Snippets
- !codeblock: codeblock with language option and title tab stops
- !link: vs code already has a snippet for link so might remove this
- !fmatter: snippet for the front matter with slug, title, authors, tags properties
- !fmatter-sidebar: snippet for the front matter with sidebar_label, and sidebar_position properties
- !admo: snippet for admonitions with type options
- !export-component: snippet for react export component with two prop options
- !import-components: snippet for react import component with name and path tabstops
- !tab: snippet for docusaurus-mdx tab with tabItem
- !element: snippet for React element

I also added a yaml.code-snippets so !authors would work
while editing in the front matter
- !author: author yaml code with name, title, url, image_url tabstops

## Requirements

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

## Installation

VS Code Market Place: [Markdown Snippets for MDX and Docusaurus](https://marketplace.visualstudio.com/items?itemName=MisterMunchkin.simple-markdown-snippets)

## Known Issues

None so far as this is still new.

## Contribution

Feel free to send a PR for any bugs or features you want to add on to this.

## Release Notes

### 0.0.5
Updated READMe.md to have better gifs and wording.

### 0.0.4
Changed name so it's clearer what the snippets are specifically for. 
- Changed README.md format a little bit

### 0.0.3

Added new logo. Pretty much copied my favorite vs code theme [Ariake Dark](https://github.com/a-wart/ariake-dark).

### 0.0.2

Initial release of simple-markdown-snippets.
Added markdown snippets used for mdx or docusaurus that aren't already built in in vs code... except for links, probably will delete that later.

### 0.0.1

Added snippets to main docusaurs, markdown, mdx code that isn't covered by vs codes built in markdown snippets.

**Enjoy!**
