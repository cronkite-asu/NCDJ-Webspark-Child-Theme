# NCDJ Webspark Child Theme

A custom WordPress child theme for the National Center on Disability and Journalism (NCDJ), built on the ASU Web Standards WordPress Theme.

> **Site-specific legacy theme:** this repository contains templates and presentation logic tailored to an existing NCDJ site. It is not a standalone theme and is unlikely to work correctly without its original parent theme, content model, menus, and widgets.

## What it contains

- A custom `blog` post type
- Templates for About, Blog archive, Contest, News, Resources, and Style Guide pages
- Dedicated widget areas for the main site sections
- ASU-specific header and navigation markup
- Site-specific styling and a Bootstrap navigation walker

## Requirements

- A WordPress installation
- The parent theme directory named `ASU-Web-Standards-Wordpress-Theme`
- The content, menus, and widgets expected by the NCDJ templates

## Installation

1. Install the required parent theme in `wp-content/themes/ASU-Web-Standards-Wordpress-Theme`.
2. Copy this repository to `wp-content/themes/NCDJ-Webspark-Child-Theme`.
3. Activate **NCDJ Webspark Child** in **Appearance → Themes**.
4. Assign the included page templates and configure the section sidebars under **Appearance → Widgets**.
5. Re-save **Settings → Permalinks** after activation so the custom Blog routes are registered.

## Development notes

The parent-theme dependency is declared by the `Template` field in [`style.css`](style.css). Changing that directory name will break child-theme loading unless the header is updated too.

This theme predates the block editor and current ASU design systems. Before deploying changes, test PHP compatibility, responsive layout, keyboard navigation, heading structure, color contrast, and all site-specific templates.

## License

GPL-2.0-or-later, as declared in [`style.css`](style.css).
