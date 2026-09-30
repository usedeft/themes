# Deft themes

One `.css` file per theme, in Settings > Appearance > Open Themes Folder. Unset tokens fall back to the base files.

## Light and dark

A theme with one mode sets `color-scheme: light` or `color-scheme: dark` on `:root`, and shows in that mode whatever Color Scheme is set to.

A theme with both modes puts each mode's tokens and rules under the `data-mode` attribute the app sets on the root, each block with its own `color-scheme`. Rules outside them apply in both modes. The Color Scheme setting then picks the mode. A mode counts only if its block is on `:root` and sets `color-scheme`: a plain `:root` block without it, beside one `data-mode` block, leaves the theme with that one mode.

Three font families are bundled: `'Inter Variable'`, `'Lilex Variable'` and `'Literata Variable'`. A theme can load its own fonts and images with a relative `url()` to files beside it.

```css
:root {
	--font-family: 'Inter Variable', sans-serif;
}
:root[data-mode='light'] {
	color-scheme: light;
	--background: #ffffff;
}
:root[data-mode='dark'] {
	color-scheme: dark;
	--background: #1e1e1e;
}
:root[data-mode='dark'] .deft-sidebar {
	--background: #181818;
}
```

Keep colors out of the plain `:root` block: a token set there and not in the dark block carries into dark mode instead of falling back to the dark base.

The app also sets `--editor-max-width` on `:root` from the Editor width setting (a length, or `100%` at Full Width) for a theme to read.

## Tokens

### Palette

- `--background`
- `--background-muted`
- `--foreground`
- `--foreground-muted`
- `--border`
- `--link`
- `--error`
- `--warning`

### Accent

- `--accent`
- `--accent-tint`
- `--accent-tint-hover`
- `--accent-foreground`: text on `--accent`

### Chrome

- `--font-family`
- `--font-family-monospace`
- `--border-radius-small`
- `--border-radius-medium`
- `--border-radius-large`
- `--icon-stroke-width`
- `--background-active`: hovered or current row
- `--overlay-background`: behind modals
- `--box-shadow-large`
- `--box-shadow-medium`
- `--box-shadow-small`

### Editor

- `--editor-font-family`
- `--editor-font-size`
- `--editor-line-height`
- `--editor-font-weight`
- `--editor-background`
- `--editor-foreground`
- `--editor-foreground-muted`
- `--editor-border`
- `--editor-background-muted`
- `--viewer-background`: behind PDFs and images

### Headings

`N` is the level, 1 to 6.

- `--heading-font-family`
- `--heading-font-weight`
- `--heading-foreground`
- `--heading-border`
- `--heading-border-width`
- `--heading-N-font-size`
- `--heading-N-font-weight`
- `--heading-N-foreground`
- `--heading-N-padding-top`
- `--heading-N-border`
- `--heading-N-border-width`

### Document

- `--highlight-background`
- `--markup-foreground`: `#`, `**` and other markers
- `--hr-border`
- `--blockquote-foreground`
- `--blockquote-font-style`
- `--blockquote-border`
- `--blockquote-border-width`
- `--code-font-family`
- `--code-font-size`
- `--code-background`
- `--code-inline-background`
- `--code-border`
- `--properties-background`: frontmatter
- `--properties-border`
- `--table-font-size`
- `--table-border`
- `--table-header-background`
- `--table-header-font-weight`
- `--table-striped-row-background`

### Syntax

- `--syntax-keyword`
- `--syntax-string`
- `--syntax-number`
- `--syntax-function`
- `--syntax-constant`
- `--syntax-type`
- `--syntax-comment`

### TeX

- `--tex-title-font-size`
- `--tex-title-font-weight`
- `--tex-title-line-height`
- `--tex-author-font-size`
- `--tex-date-font-size`
- `--tex-date-foreground`
- `--tex-caption-font-size`
- `--tex-caption-font-style`
- `--tex-caption-foreground`
- `--tex-script-font-size`

## Classes

Classes take tokens too, for just that part. No `!important` needed, except on the find bar, whose own rules outrank a theme's: set tokens on `.deft-popover` there, or scope the rule under `:root[data-mode]`.

### Window

- `.deft-app`
- `.deft-workspace`: top border is the rule under the title bar (Windows, macOS)
- `.deft-sidebar`
- `.deft-sidebar-left`
- `.deft-sidebar-right`
- `.deft-toolbar`
- `.deft-spacer`: the gap pushing a bar's later items to its far end
- `.deft-statusbar`
- `.deft-sync-footer`: the sync row under the file tree
- `.deft-main`: holds `.deft-editor` and its corner buttons, so size this to narrow the editor
- `.deft-editor-buttons`: the corner buttons; `--editor-overlay-width` is their width
- `.deft-editor`

### Note

- `.deft-breadcrumbs`
- `.deft-note-title`

### File tree

- `.deft-tree`: `.drag-over` while a drag would drop into the top level
- `.deft-tree-row`: `.selected` when open, `.drag-over` while a drag would drop into it
- `.deft-tree-folder`
- `.deft-tree-project`
- `.deft-tree-file`

### Panels

- `.deft-panel`
- `.deft-outline`
- `.deft-backlinks`
- `.deft-tasks`
- `.deft-bookmarks`
- `.deft-problems`
- `.deft-panel-item`: `.active` current heading, `.done` checked task

### Controls

- `.deft-tab`: `.active` when shown
- `.deft-icon-button`: `.active` when toggled
- `.deft-button`
- `.deft-button-primary`
- `.deft-input`

### Popovers and modals

- `.deft-popover`: menus, find panel, tooltips, viewer controls
- `.deft-find`
- `.deft-menu`
- `.deft-menu-item`
- `.deft-modal`
- `.deft-settings`
- `.deft-settings-page`
- `.deft-search`
