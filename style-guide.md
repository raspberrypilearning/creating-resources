## Style Guide

### Headings

The page title should be given as a top level heading, and this should be the only top level heading on the page.

Second level headings should reflect the sections of the document, and third level headings should be used for subheadings under these sections. Use further headings hierarchically if needed.

### Emphasis

Strong emphasis (bold) should not be used as headings. Use headings. Only use bold or italics to emphasise a word or some words in a sentence, as appropriate.

### Lists

#### Unordered lists

Always use a single hyphen followed by a single space, optionally with a line space between each item (for longer items).

#### Ordered lists

Always precede each list item with a `1.` and allow automatic numbering to take effect. This makes it easier for collaborators to add list items in the middle without having to renumber them.

#### Nested lists

Use four spaces to indent a sub-list.

#### Paragraphs in between list items

If you need to include further text in between list items, indent the text with four spaces. This will allow your list to continue (i.e. numbering in an ordered list will not break sequence). Ensure list numbering is not unintentionally broken.

### Links

Use links as described above. Check relative links are correct and be sure to update them if you change file or folder names or move files to a new location.

#### Relative links with a leading slash

You may be familiar with the use of a leading `/` to link relatively from the root, i.e. the path `/worksheet.md` would always point at the `worksheet.md` file at the root of the repository, rather than use a series of `../` to go back the correct number of levels.

This is a useful and valid technique, however as resources are copied on to the Raspberry Pi website, the leading `/` would refer to the root of the website, not the root of the project. Therefore it is advised you only use relative links with `../`.

### Images

It is good practice to have an `images` folder in the root of the repository which contains all the images used in the project. Then refer to images relatively when you include them in a document.

For larger projects, you may wish to use an `image` folder in each folder inside the repository. For example on a scheme of work if you have a folder containing each lesson's documents and assets, you may wish to keep images used in each lesson in their respective `image` folders.

Note that GitHub does not currently support uploading of images, so you would have to use a git client on your PC rather than directly in the browser.

### Code blocks

Use code blocks! Use syntax highlighting where possible! Both GitHub and the Raspberry Pi website supports many languages. Be sure to use the correct language alias - common ones are `python`, `ruby`, `php`, `bash` and `javascript`.

#### Inline code blocks

It's recommended you use inline code blocks for language keywords, code snippets and some technical things like package names, e.g. "Install the package `python-picamera` to access the camera directly from Python."

### Block quotes

### Tables

### Horizontal rule

### Line breaks

### Anchors

## Alternatives

There are alternative methods to achieving the required formatting to the methods shown in this document. Purposely these have been left out here as we would prefer those writing materials for our use follow the same format to make collaboration and editing easier for all.
