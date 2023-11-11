# Markdown

## [My Markdown Syntax Reference](https://github.com/chrisrobles/markdown-cheatsheet/blob/main/markdown-syntax.md?plain=1)

<br>

[Common Mistakes](https://gist.github.com/DavidAnson/006a6c2a2d9d7b21b025)

[GitHub's Extended Syntax Reference](https://www.markdownguide.org/extended-syntax)

## Link Tricks

- Header in current file
  - `[text](#_some-header)`
- To another file
  - `[text](/path/to/file.md)`
- Header in another file
  - `[text](otherFile.md#other-header)`
- Ref links (links saved in variable)
  [link-id]: https://www.google.com
  `[text][link-id]`
- Create vscode link validation exceptions
  - In settings.json add "markdown.validate.ignoredLinks"

## VSCode

### Change default editor

1) Right click file
2) Click `Open with...`
3) Click `Change default editor` at the bottom of the pop up

### [Tips](https://code.visualstudio.com/Docs/languages/markdown#_markdown-preview)

- Rename markdown headers and all its links: right click header -> `Rename symbol`
- Paste link on selected text for link auto format
- `> Create table of contents` auto creates table of contents for file
- Change styling of markdown preview
  
  ```json
  "markdown.styles": [
        "/home/chris/Documents/Code/current/markdown-preview.css", //Linux
        "C:\\Users\\chris\\Documents\\Code\\current\\markdown-preview.css" //Windows
    ],
  ```

### Keyboard Shortcuts

- Open preview `ctrl+shift+v`
<br>
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
