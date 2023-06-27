# Markdown

- [Markdown](#markdown)
  - [Heading {#custom-id}](#heading-custom-id)
  - [Tables](#tables)
    - [Table of contents](#table-of-contents)
  - [Link Tricks](#link-tricks)
  - [VSCode](#vscode)
    - [Tips](#tips)
    - [Keyboard Shortcuts](#keyboard-shortcuts)
  - [Extensions](#extensions)
  - [Extra Links to Look At](#extra-links-to-look-at)

[Common Mistakes](https://gist.github.com/DavidAnson/006a6c2a2d9d7b21b025)
[Github Cheat Sheet](https://www.markdownguide.org/extended-syntax)

--- horizontal rule

## Heading {#custom-id}

*italics* **bold** ~~strikethrough~~ <mark>highlight</mark> ==highlight==
_italics_ __bold__ <- useful for nesting bold and italics
:yellow_heart:

\*escaped the\*

> Text that is a quote
>
> > Nested

```js
// Code Blocks
console.log("hello world");
```

`Code Blocks`

<christian@aol.com>
<https://www.google.com>

1. Ordered
2. List

- List
  - nested list
    added paragraph

term
: definition

- [ ] Check
- [x] boxes

`rgb(233,32,112)`

<!-- This content will not appear in the rendered Markdown -->

---

FILES AND URLS
[text](file path / url 'accessibility alt text')

IMAGES
![alt text](20230521195745.png "hover / screen reader")

Sentence links to a footnote [^1]

[^1]: Foot note

---

## Tables

Table prettify `alt+shift+f` `ctrl+shift+i` linux

| Header     | Header | Header |
| :--------- | :----: | -----: |
| Left       | Middle |  Right |
| \| escaped |

Cant include :

- Headings
- Blockquotes
- Horizontal rules
- Images
- Lists
- HTML tags
- Code blocks

### Table of contents

`> Create table of contents`

### Not in table of contents <!-- omit from toc -->

## Link Tricks

- Header in current file
  - `[text](#_some-header)`
- To another file
  - `[text](/path/to/file.md)`
- Creating links to a header in another file
  - `[text](otherFile.md#other-header)`
- Ref links (links saved in variable)
  [link-id]: https://www.google.com
  `[text][link-id]`
- Create vscode link validation exceptions
  - In settings.json add "markdown.validate.ignoredLinks"

## VSCode

### [Tips](https://code.visualstudio.com/Docs/languages/markdown#_markdown-preview)

- Rename markdown headers and all its links w/ vscode `Rename symbol`
- Paste link on selected text
- Change styling of markdown preview
  
  ```json
  "markdown.styles": [
        "/home/chris/Documents/Code/current/markdown-preview.css", //Linux
        "C:\\Users\\chris\\Documents\\Code\\current\\markdown-preview.css" //Windows
    ],
  ```

### Keyboard Shortcuts

- Go to header in file `ctrl+shift+o`
- Bold `ctrl+b`
- Check mark `alt+c`
  <br>
- Quick change to bullets `ctrl+m ctrl+b`
- Quick change to numbers `ctrl+m ctrl+1`
- Quick change to checkboxes `ctrl+m ctrl+x`

## Extensions

*__NOTE:__* VSCode already comes with a markdown preview and editor.

- Markdown Extension Pack (bat67.markdown-extension-pack)
  Includes:
  - Markdown All in One
  - Markdown Checkboxes
  - Markdown Emoji
  - Markdown Paste
  - Markdown Pdf
  - Markdown Preview Enhanced
  - Markdown Preview GitHub Styling
  - Markdown Shortcuts
  - Markdown Table Prettifier
  - Markdown+Math
  - markdownlint
    - enforces a library of rules to encourage standards and consistency for Markdown files
    - helps prevent [common markdown mistakes](https://gist.github.com/DavidAnson/006a6c2a2d9d7b21b025)
    - Can have VSCode ignore certain rules in settings.json
      - `"markdownlint.config": {"MD033": false,},`

## Extra Links to Look At

<https://daringfireball.net/projects/markdown/basics>

<https://daringfireball.net/projects/markdown/dingus>

<https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links>
