Best viewed on the website: <https://rumovz.github.io/anki-manual-de_DE>

This manual is licensed under the CC BY-SA 4 license:

<https://creativecommons.org/licenses/by-sa/4.0/>

Pull requests are welcome (see below). Unless you state otherwise, any pull requests you
submit will be licensed under the above license.

<hr>

# Contributing

Contributions can be made in three ways.

1. **Translating a file.**
    Please see [#1](https://github.com/RumovZ/anki-manual-de_DE/issues/1) and
    [conventions](#conventions) below.

2. **Improving an existing translation.**
    A simple PR will do, but please see [conventions](#conventions) below.

3. **Incorporating updates from the official manual.**
    To ensure synchronisation with the official manual, updates to it will be handled
    by the maintainers, until a reasonable workflow has been decided on.
    More extensive updates may be incorporated as-is (in English), and issues opened
    for the new untranslated parts.

## Conventions

### Format

This list of conventions is to ensure easier synchronisation with the official manual,
cleaner merges, and a consistent look.

- Empty lines, heading placements, etc. in the official manual are to be preserved
  as much as possible. Single linebreaks (which are ignored in Markdown) may be
  used to the heart's content.
- File names are not to be translated. Title translations are made in `SUMMARY.md`
  (in square brackets) and have to agree with the titles on the relevant pages.
- Linebreaks should be inserted roughly after at most 100 characters.
- Formatting, such as \` for code and `<kbd></kbd>` for key presses, may be
  improved, as it's not consistent in the official manual.

### Translation

This list of conventions is to ensure a minimum of consistency within the manual.
If you disagree with or want to add anything, feel free to open an issue.

- Use "du" over "Sie".
- Anglicisms are to be avoided. (Of course, that's quite often impossible.)
- Translations should sound natural. Don't hesitate to deviate from the original,
  as long as the content remains the same. Updates to the content, however, must be
  made on <https://github.com/ankitects/anki-manual> before they can be integrated
  here.
- Ideally, terms used in Anki should agree with the translations over on
  <https://i18n.ankiweb.net/de/>. Of course, improvements can be made there as well.

## Tips

### Previewing Changes

If you want to preview your local changes, you can install
[mdbook](https://github.com/rust-lang/mdBook),
put it in your `PATH`, and run `mdbook serve -o` from within your repository folder.
The binaries and a more detailed description can be found under the link above.
In order to render the table of contents at the top of some pages,
[mdbook-toc](https://github.com/badboy/mdbook-toc) is needed as well, but this
requires a Rust installation.
