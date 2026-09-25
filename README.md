# Tokyo Night

A [fulgurite](https://github.com/fulgurite-plugin) theme: [Tokyo Night](https://github.com/folke/tokyonight.nvim)'s night style (bg_dark1 · bg_dark · bg · bg_highlight).

A whole theme: flat colors for the window, the sidebar, the note list and the paper, and its own text colors. Choose it under Settings › Theme › Interface.

## Install

In fulgurite: Settings › Theme › Available Themes › Install. Updates show there too.

## Making a theme

A theme is a repository like this one: `package.json` says `"theme": true`, and `theme.json` holds the colors
(`#RRGGBB` or `#RRGGBBAA`; JSON5, so comments are fine):

- `name`, and `appearance`: `light` or `dark`
- `interface` (`window` `sidebar` `noteList` `paper`): a whole theme. Leave it out for a text theme
- `text` (`text` `heading` `link` `tag` `quote` `muted` `code`): the editor's colors

`npm version patch` releases it: the version goes up, and the tag `v<version>` is made and pushed. To list a theme in the
app, open a pull request adding its repository to `themes.json` in
[fulgurite-registry](https://github.com/fulgurite-plugin/fulgurite-registry).

Colors after folke/tokyonight.nvim, Apache-2.0.
