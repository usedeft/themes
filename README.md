# Theming Deft

Three font families are bundled: `'Inter Variable'`, `'Lilex Variable'` and `'Literata Variable'`. A theme can load its own fonts and images with a relative `url()` to files beside it.

```css
:root {
	--font-family: 'Inter Variable', sans-serif;
}
```

## Light and dark

```css
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
- `--accent-foreground`

### Chrome

- `--font-family`
- `--font-family-monospace`
- `--border-radius-small`
- `--border-radius-medium`
- `--border-radius-large`
- `--icon-stroke-width`
- `--background-active`
- `--overlay-background`
- `--box-shadow-large`
- `--box-shadow-medium`
- `--box-shadow-small`

### Editor

- `--editor-max-width`
- `--editor-overlay-width`
- `--editor-font-family`
- `--editor-font-size`
- `--editor-line-height`
- `--editor-font-weight`
- `--editor-background`
- `--editor-foreground`
- `--editor-foreground-muted`
- `--editor-border`
- `--editor-background-muted`
- `--viewer-background`


### Headings

`N`: Heading level 1 to 6

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
- `--markup-foreground`
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
- `--properties-background`
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

### Window

- `.deft-app`
- `.deft-touch`
- `.deft-phone`
- `.deft-workspace`
- `.deft-sidebar`
- `.deft-sidebar-left`
- `.deft-sidebar-right`
- `.deft-toolbar`
- `.deft-spacer`
- `.deft-statusbar`
- `.deft-sync-footer`
- `.deft-main`
- `.deft-editor`
- `.deft-editor-buttons`

### Note

- `.deft-breadcrumbs`
- `.deft-note-title`

### File tree

- `.deft-tree`
- `.deft-tree.drag-over`
- `.deft-tree-row`
- `.deft-tree-row.selected`
- `.deft-tree-row.drag-over`
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
- `.deft-panel-item`
- `.deft-panel-item.active`
- `.deft-panel-item.done`

### Controls

- `.deft-tab`
- `.deft-tab.active`
- `.deft-icon-button`
- `.deft-icon-button.active`
- `.deft-button`
- `.deft-button-primary`
- `.deft-input`

### Popovers and modals

- `.deft-popover`
- `.deft-find`
- `.deft-menu`
- `.deft-menu-item`
- `.deft-modal`
- `.deft-settings`
- `.deft-settings-page`
- `.deft-search`
