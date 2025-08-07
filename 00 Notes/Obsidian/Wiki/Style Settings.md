---
Type: Note
---
# `= this.file.link`
>[!Properties]- |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` 
>Version:: 3
>Parent:: [[Plugins]]
>Tags:
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
# Body:
Edit some CSS file from inside of Obsidian
- Theme 
- Supercharged Links


# Backup

```
{
  "minimal-advanced@@styled-scrollbars": false,
  "minimal-advanced@@cursor": "default",
  "minimal-style@@title-color@@dark": "#000000",
  "minimal-style@@minimal-unstyled-tags": false,
  "minimal-style@@tag-radius": "4px",
  "minimal-style@@tag-background@@dark": "#24262A",
  "minimal-style@@color-red@@dark": "#B34646",
  "minimal-style@@h1-l": true,
  "minimal-style@@h2-l": true,
  "minimal-style@@h4-size": "1.1em",
  "minimal-style@@h4-variant": "normal",
  "minimal-style@@h5-size": "1.1em",
  "minimal-style@@h5-variant": "normal",
  "minimal-style@@h6-size": "1.1em",
  "minimal-style@@h6-variant": "normal",
  "minimal-style@@image-muted": 1,
  "minimal-style@@maximize-tables-off": "maximize-tables-off",
  "minimal-style@@row-lines": true,
  "minimal-style@@sidebar-tabs-style": "sidebar-tabs-default",
  "minimal-style@@mobile-left-sidebar-width": 280,
  "minimal-style@@table-nowrap": true,
  "minimal-style@@h2-size": "1.1em",
  "minimal-style@@bg1@@light": "#494141",
  "minimal-style@@bg1@@dark": "#24262A",
  "minimal-style@@tag-border-width": "1px",
  "minimal-style@@h3-l": true,
  "minimal-style@@h2-color@@dark": "#FC9402",
  "minimal-style@@h2-style": "normal",
  "minimal-style@@h3-color@@dark": "#73A262",
  "minimal-style@@h1-color@@dark": "#B3324A",
  "minimal-style@@h1-weight": 600,
  "minimal-style@@h4-color@@dark": "#117A3F",
  "minimal-style@@h5-color@@dark": "#D2D149",
  "minimal-style@@h6-color@@dark": "#D348DB",
  "minimal-style@@h6-weight": 600,
  "minimal-style@@h5-weight": 600,
  "minimal-style@@h4-weight": 600,
  "minimal-style@@active-line-on": false,
  "minimal-style@@active-line-bg@@dark": "#230627",
  "minimal-style@@h3-size": "1.1em",
  "anuppuccin-theme-settings@@anuppuccin-theme-dark": "ctp-macchiato",
  "anuppuccin-theme-settings@@anuppuccin-light-theme-accents": "none",
  "anuppuccin-theme-settings@@anuppuccin-theme-accents": "ctp-accent-green",
  "anuppuccin-theme-settings@@anp-speech-bubble": false,
  "anuppuccin-theme-settings@@anp-custom-checkboxes": false,
  "anuppuccin-theme-settings@@anp-alt-rainbow-style": "anp-full-rainbow-color-toggle",
  "anuppuccin-theme-settings@@anp-rainbow-file-toggle": false,
  "anuppuccin-theme-settings@@anp-full-rainbow-text-color-toggle-light": false,
  "modular-css-layout-wv@@narrow-max-width": "8500px",
  "obsidian-prism-theme@@pt-disable-blur": false,
  "obsidian-prism-theme@@pt-disable-callout-styling": true,
  "obsidian-prism-theme@@pt-disable-mark-highlight-styling": true,
  "obsidian-prism-theme@@pt-collapsed-pinned-tab": false,
  "obsidian-prism-theme@@pt-pdf-dark-theme": false,
  "obsidian-prism-theme@@color-schemes-dt": "pt-color-scheme-mocha-dt",
  "obsidian-prism-theme@@accent-style-dt": "pt-accent-style-borderandfilled-dt",
  "obsidian-prism-theme@@dark-accent-color-preset": "pt-accent-color-custom-dt",
  "obsidian-prism-theme@@highlight-text-accent-dt": "pt-highlight-text-custom-dt",
  "obsidian-prism-theme@@pt-custom-vault-banner": false,
  "obsidian-prism-theme@@file-line-width": 700,
  "obsidian-prism-theme@@graph-fill-color-lt": "var(--color-grey-text)",
  "obsidian-prism-theme@@graph-fill-custom-color-lt": "#174675",
  "obsidian-prism-theme@@color-scheme-style-lt": "pt-color-scheme-style-two-tone-and-border-lt",
  "obsidian-prism-theme@@accent-style-lt": "pt-accent-style-minimal-lt",
  "obsidian-prism-theme@@light-accent-color-preset": "pt-accent-color-purple-lt",
  "obsidian-prism-theme@@highlight-text-accent-lt": "pt-highlight-text-accent-lt",
  "obsidian-prism-theme@@light-mark-highlight-text-color-preset": "pt-highlight-text-color-lt",
  "obsidian-prism-theme@@light-mark-highlight-style": "pt-highlight-style-borderandfilled-lt",
  "obsidian-prism-theme@@radius-m": 8,
  "obsidian-prism-theme@@radius-s": 4,
  "obsidian-prism-theme@@left-sidebar-tab-label-alignment": "pt-tab-label-left-sidebar-center",
  "obsidian-prism-theme@@right-sidebar-tab-label-alignment": "pt-tab-label-right-sidebar-center",
  "obsidian-prism-theme@@nav-header-left-sidebar-position": "pt-nav-header-left-sidebar-position-top",
  "obsidian-prism-theme@@nav-header-left-sidebar-alignment": "pt-nav-header-left-sidebar-align-center",
  "obsidian-prism-theme@@nav-header-right-sidebar-position": "pt-nav-header-right-sidebar-position-top",
  "obsidian-prism-theme@@tab-header-alignment": "pt-tab-header-left",
  "obsidian-prism-theme@@pt-file-explorer-folder-icon": true,
  "obsidian-prism-theme@@pt-file-explorer-folder-icon-color": "pt-file-explorer-folder-icon-default",
  "obsidian-prism-theme@@pt-titlebar-hide-text": false,
  "obsidian-prism-theme@@pt-status-bar-style": "pt-status-bar-position-fixed",
  "obsidian-prism-theme@@pt-fixed-status-bar-align": "pt-fixed-status-bar-align-right",
  "obsidian-prism-theme@@status-bar-preset-lt": "pt-status-bar-default-lt",
  "obsidian-prism-theme@@status-bar-text-color-lt": "pt-status-bar-text-dark-lt",
  "obsidian-prism-theme@@scroll-bar-size": 16,
  "obsidian-prism-theme@@pt-fade-inactive-tabs": false,
  "obsidian-prism-theme@@inline-title-color-lt": "var(--text-normal)",
  "obsidian-prism-theme@@color-schemes-lt": "pt-color-scheme-swan-lt",
  "obsidian-prism-theme@@color-scheme-style-dt": "pt-color-scheme-style-two-tone-and-border-dt",
  "obsidian-prism-theme@@highlight-text-accent-custom-dt": "#000000",
  "obsidian-prism-theme@@color-accent-base-dt": "#1F2B47",
  "obsidian-prism-theme@@color-accent-text-dt": "#6D4DC6",
  "obsidian-prism-theme@@color-accent-tint-dt": "#4D62A9",
  "grubbed@@collapsed-borders": false,
  "grubbed@@show-sidebar-tabs": true,
  "grubbed@@show-titlebar": true,
  "grubbed@@show-scrollbar": false,
  "grubbed@@status-bar-border": true,
  "entry-point@@smooth-mode": false,
  "entry-point@@minimal-mode": false,
  "entry-point@@minimal-sidebar": "sidebar-hide",
  "entry-point@@color-scheme-selector": "color-scheme-default",
  "entry-point@@separate-color-scheme": false,
  "entry-point@@floating-sides": false,
  "supercharged-links@@eb73-e7b3-color": "#E53935",
  "supercharged-links@@eb73-e7b3-weight": "bold",
  "supercharged-links@@59a7-8d8c-before": "🎥",
  "supercharged-links@@1353-12e6-color": "#BF8418",
  "supercharged-links@@9630-e603-before": "💡",
  "supercharged-links@@313f-b37d-before": "🛠️",
  "supercharged-links@@4cdf-9a90-before": "⭐",
  "supercharged-links@@12fc-dbdc-before": "🚩",
  "supercharged-links@@0822-46b3-before": "🔗",
  "supercharged-links@@a34d-403b-color": "#FB8C00",
  "supercharged-links@@532a-edfd-color": "#FDD835",
  "supercharged-links@@bfe3-f2ed-color": "#43A047",
  "supercharged-links@@249b-4724-color": "#1E88E5",
  "supercharged-links@@cbb1-720e-color": "#8E24AA",
  "supercharged-links@@bee7-0118-color": "#EC407A",
  "supercharged-links@@cc7b-82b0-color": "#6D4C41",
  "supercharged-links@@f5ae-b583-color": "#9E9E9E",
  "supercharged-links@@5575-2e32-color": "#212121",
  "supercharged-links@@495f-d2a0-color": "#FF4B4B",
  "supercharged-links@@495f-d2a0-weight": "bold",
  "supercharged-links@@1353-12e6-weight": "bold",
  "supercharged-links@@8f0a-6764-weight": "bold",
  "supercharged-links@@495f-d2a0-decoration": "initial",
  "supercharged-links@@8f0a-6764-color": "#648F0B",
  "supercharged-links@@bee7-0118-weight": "bold",
  "supercharged-links@@a34d-403b-weight": "bold",
  "supercharged-links@@532a-edfd-weight": "bold",
  "supercharged-links@@bfe3-f2ed-weight": "bold",
  "supercharged-links@@249b-4724-weight": "bold",
  "supercharged-links@@cbb1-720e-weight": "bold",
  "supercharged-links@@cc7b-82b0-weight": "bold",
  "supercharged-links@@f5ae-b583-weight": "bold",
  "supercharged-links@@5575-2e32-weight": "bold"
}
```





# Foot
```meta-bind-embed
[[Foot note]]
``` 