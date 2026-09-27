
# Theming Deft

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

`N` 1 to 6

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

You can use tokens with classes.

### Window

- `.deft-app`
- `.deft-workspace`
- `.deft-sidebar`
- `.deft-sidebar-left`
- `.deft-sidebar-right`
- `.deft-toolbar`
- `.deft-statusbar`
- `.deft-editor`

### Note

- `.deft-breadcrumbs`
- `.deft-note-title`

### File tree

- `.deft-tree`
- `.deft-tree-row`: `.selected` when open
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
- `.deft-menu`
- `.deft-menu-item`
- `.deft-modal`
- `.deft-settings`
- `.deft-settings-page`
- `.deft-search`
