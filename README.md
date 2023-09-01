# Markdown Extension Pack

This extension pack packages some of the most popular Markdown extensions.

此擴展包打包了一些最流行的 Markdown 擴展。

## Extensions Included

### Linting Tool

- [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)

  Markdown linting and style checking for Visual Studio Code. Check [Rules](https://github.com/DavidAnson/markdownlint/blob/main/doc/Rules.md) for more details.

  When you get rule violations (wavy underlined text) in a doc, it support **Quick Fix**.

  Useful Shortcuts:

  - Windows
    - `Ctrl + .` : Quick Fix
  - macOS
    - `⌘ + .` : Quick Fix

  > I use [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) to validate my Markdown files. But some of the rules might break your content by accident if you enabled **Editor: Format On Save** (`editor.formatOnSave`) setting. Below is my `.markdownlint.json` file which disabled some rules that I don't need. Especially the [MD044 - Proper names should have the correct capitalization](https://github.com/DavidAnson/markdownlint/blob/main/doc/Rules.md#md044---proper-names-should-have-the-correct-capitalization) might broken some of the **Terms** in your doc.

  ```json
  {
    "MD001": false,
    "MD012": false,
    "MD013": false,
    "MD028": false,
    "MD034": false,
    "MD041": false,
    "MD044": false,
    "MD029": {
      "style": "ordered"
    }
  }
  ```

### Editing Tools

- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)

  Useful Shortcuts:

  - Windows
    - `Ctrl + B` : Toggle bold; 切換粗體
    - `Ctrl + I` : Toggle italic; 切換斜體
    - `Alt + S` : Toggle strikethrough; 切換刪除線
    - `Alt + C` : Check/Uncheck task list item; 選中/取消選中任務列表項
    - `Ctrl + Shift + ]` : Toggle heading (uplevel); 切換標題（上層）
    - `Ctrl + Shift + [` : Toggle heading (downlevel); 切換標題（下層）
    - `Alt + Shift + F` : Format Document with a Table formatter; 使用表格格式化程序格式化文檔
  - macOS
    - `Alt + C` : Check/Uncheck task list item
    - `Cmd + B` : Toggle bold
    - `Cmd + I` : Toggle italic
    - `Cmd + Shift + ]` : Toggle heading (uplevel)
    - `Cmd + Shift + [` : Toggle heading (downlevel)
    - `Alt + Shift + F` : Format Document with a Table formatter

- [Markdown Paste](https://marketplace.visualstudio.com/items?itemName=telesoho.vscode-markdown-paste-image)

  Useful Shortcuts:

  - `Ctrl + Alt + V` : Simply copy a image to Clipboard then use `Ctrl+Alt+V` to paste into your doc.\
    (只需將圖像複製到剪貼板，然後使用 `Ctrl + Alt + V` 粘貼到文檔中即可。)

    > You can paste not only images, but also any Text, HTML, Rich-Text to Markdown.\
    > (您不僅可以粘貼圖像，還可以將任何文本，HTML，富文本粘貼到 Markdown。)

- [Markdown Paste Image](https://marketplace.visualstudio.com/items?itemName=onesdev.vscode-paste-image-plus)

- [Excel to Markdown table](https://marketplace.visualstudio.com/items?itemName=csholmq.excel-to-markdown-table)

  Useful Shortcuts:

  - `Shift + Alt + V` : Copy a region of Excel Spreadsheet then use `Shift+Alt+V` to paste into a markdown doc in a table from.\
  (複製 Excel 電子表格的一個區域，然後使用 `Shift + Alt + V` 粘貼到表格中的 Markdown 文檔中。)

- [CSV to Markdown Table Converter](https://marketplace.visualstudio.com/items?itemName=Marchiore.csvtomarkdown)

   Paste CSV to Markdown doc. Select the corresponding text to CSV. Hit `F1` and select **Convert CSV to Markdown Table** command. Done!\
   (將 CSV 粘貼到 Markdown 文檔。 選擇 CSV 中對應的文本。 按 `F1` 並選擇 **將 CSV 轉換為 Markdown 表** 命令。 完畢！)

### Markdown Preview enhancements

- [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles)

  Changes VS Code's built-in markdown preview to match GitHub's styling.\
  (更改 VS Code 的內置 Markdown 預覽以匹配 GitHub 的樣式。)

- [Markdown Image Size](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-image-size)

  Adds `![](IMAGEURL =100x200)` image size syntax support to VS Code's built-in Markdown preview.\
  (向 VS Code 的內置 Markdown 預覽添加 `![](IMAGEURL =100x200)` 圖像大小語法支持。)

  > Azure DevOps's Wiki page support [resize image](https://docs.microsoft.com/en-us/azure/devops/project/wiki/markdown-guidance?view=azure-devops&WT.mc_id=DT-MVP-4015686#images) syntax.

- [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid)

  Adds [Mermaid](https://mermaid-js.github.io/mermaid/) diagram and flowchart support to VS Code's builtin markdown preview\
  (為 VS Code 的內置 Markdown 預覽添加 [Mermaid](https://mermaid-js.github.io/mermaid/) 圖表和流程圖支持)

  It support both `::: mermaid` and ` ```mermaid ` syntax.

  > Azure DevOps's Wiki page [support Mermaid diagram](https://docs.microsoft.com/en-us/azure/devops/project/wiki/wiki-markdown-guidance?view=azure-devops&WT.mc_id=DT-MVP-4015686#add-mermaid-diagrams-to-a-wiki-page) syntax.

- [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)

  Adds [:emoji:](https://www.webpagefx.com/tools/emoji-cheat-sheet/) syntax support to VS Code's built-in Markdown preview.\
  (向 VS Code 的內置 Markdown 預覽添加 [:emoji:](https://www.webpagefx.com/tools/emoji-cheat-sheet/) 語法支持。)

- [Markdown yaml Preamble](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-yaml-preamble)

  Renders YAML front matter as a table in the built-in markdown preview.\
  (在內置 Markdown 預覽中將 YAML 前面的內容呈現為表格。)

- [Markdown Footnotes](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-footnotes)

  Adds `[^1]` footnote syntax support to VS Code's built-in Markdown preview\
  (向 VS Code 的內置 Markdown 預覽添加 `[^1]` 腳註語法支持)

### Misc. Utilities

- [Copy Markdown as HTML](https://marketplace.visualstudio.com/items?itemName=jerriepelser.copy-markdown-as-html)

  I'll turn markdown into HTML and put it onto Clipboard. No file will be generated. It is very useful that when I writing posts.\
  (我會將 Markdown 轉換為 HTML 並將其放入剪貼板。 不會生成任何文件。 當我寫帖子的時候，這非常有用。)

- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

  You can right-click on any folder in the **EXPLORER** pane and choose **Generate .editorconfig** command.\
  (您可以右鍵單擊 **EXPLORER** 窗格中的任何文件夾，然後選擇 **Generate .editorconfig** 命令。)

  ```ini
  root = true

  [*]
  indent_style = space
  indent_size = 4
  end_of_line = crlf
  charset = utf-8
  trim_trailing_whitespace = true
  insert_final_newline = false

  [*.md]
  indent_size = 2
  ```

- [Markdown Extended](https://marketplace.visualstudio.com/items?itemName=jebbs.markdown-extended)
- [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf)

  **Usage**\
  **Command Palette**
  1. Open the Markdown file
  2. Press `F1` or `Ctrl+Shift+P`
  3. Type export and select below
      - markdown-pdf: Export (settings.json)
      - markdown-pdf: Export (pdf)
      - markdown-pdf: Export (html)
      - markdown-pdf: Export (png)
      - markdown-pdf: Export (jpeg)
      - markdown-pdf: Export (all: pdf, html, png, jpeg)

![](images/usage1.gif)

  **Menu**
  1. Open the Markdown file
  2. Right click and select below
      - markdown-pdf: Export (settings.json)
      - markdown-pdf: Export (pdf)
      - markdown-pdf: Export (html)
      - markdown-pdf: Export (png)
      - markdown-pdf: Export (jpeg)
      - markdown-pdf: Export (all: pdf, html, png, jpeg)

![](images/usage2.gif)

### Customizable Shortcuts

1. **Insert Snippet** (`editor.action.insertSnippet`)

   `Ctrl + K` : Insert Link on selected text\
   (在選定的文本上插入鏈接)

   > Your can just paste link from clipboard on selected text if you installed [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) extension which is already included in this extension pack.\
   > (如果您安裝了[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) 擴展程序，您只需將剪貼板中的鏈接粘貼到所選文本上即可，該擴展程序已包含在這個擴展包。)

2. **Snippets for Markdown** (`editor.action.triggerSuggest`)

   `Ctrl + Space` : Trigger suggest; 觸發建議

3. **Markdown: Open Preview** (`markdown.showPreview`)

   I'll remove the built-in `Ctrl + Shift + V` for this command. There is another shortcut registered below:\
   (我將刪除此命令的內置 `Ctrl + Shift + V`。 下面註冊了另一個快捷方式：)

   `Ctrl + Shift + Alt + P` : Open Preview

4. **Markdown: Open Preview to the side** (`markdown.extension.togglePreview`)

   The default `Ctrl + K V` will not available if your installed [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one). So you have to customize the built-in Keyboard Shortcuts to `Ctrl + Shift + V`.\
   (如果您安裝了[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)，則預設的 `Ctrl + K V` 將不可用。 因此，您必須將內置鍵盤快捷鍵自定義為 `Ctrl + Shift + V`。)

   `Ctrl + Shift + V` : Open Preview to the side (The 2nd editor)\
   (打開側面預覽（第二個編輯器）)

   > You can hit the same hotkey to close the Preview.\
   > (您可以點擊相同的熱鍵來關閉預覽。)

### Extensions NOT Included but might be useful

You need to install the following extensions manually if you need:\
(如果需要，您需要手動安裝以下擴展：)

- [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)

  Markdown Preview Enhanced is an extension that provides you with many useful functionalities such as automatic scroll sync, [math typesetting](https://shd101wyy.github.io/markdown-preview-enhanced/#/math), [mermaid](https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams?id=mermaid), [PlantUML](https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams?id=plantuml), [pandoc](https://shd101wyy.github.io/markdown-preview-enhanced/#/pandoc), PDF export, [code chunk](https://shd101wyy.github.io/markdown-preview-enhanced/#/code-chunk), [presentation writer](https://rawgit.com/shd101wyy/markdown-preview-enhanced/master/docs/presentation-intro.html), etc. A lot of its ideas are inspired by [Markdown Preview Plus](https://github.com/atom-community/markdown-preview-plus) and [RStudio Markdown](http://rmarkdown.rstudio.com/).

- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

  There is a **Format Document (Forced)** command (`prettier.forceFormatDocument`) that can format your Markdown document by force!

  I'll bind `Ctrl + Alt + Shift + F` hotkey to this command.

- [Markdown+Math](https://marketplace.visualstudio.com/items?itemName=goessner.mdmath)

  If you want to use this extension, please remember disable `math.enabled` option.

- [Medium to Markdown](https://marketplace.visualstudio.com/items?itemName=moshfeu.vscode-medium-to-markdown)

  Import your Medium posts into Markdown in your editor.

- [Front Matter CMS](https://marketplace.visualstudio.com/items?itemName=eliostruyf.vscode-front-matter)

### Code Snippets

| Prefix    | Description                         |
| --------- | ----------------------------------- |
| ` ``` `   | fenced code blocks                  |
| `details` | Use `<details>` element in Markdown |

### Useful links

- [Markdown and Visual Studio Code](https://code.visualstudio.com/Docs/languages/markdown)
- [你一定不能不知道的 Markdown 寫作技巧](https://www.youtube.com/watch?v=_05BEggK0IU)
- [你一定不能不知道的 Markdown 寫作技 - slideshare](https://www.slideshare.net/WillHuangTW/learn-markdown-authoring-skills)
- [Markdown 技術文件寫作 - VSCode FrontMatter 擴充套件](https://blog.darkthread.net/blog/vscode-frontmatter-ext/)

**Enjoy!**
