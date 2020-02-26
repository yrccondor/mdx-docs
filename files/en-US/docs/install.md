# Install, Upgrade & Uninstall

## Installation

MDx is not currently on the WordPress official theme library. You need to manually download MDx and install it.

Once you have get the installation package, you only need to open the WordPress admin panel and upload the installation package according to the instruction on the page. After the installation, you can activate MDx and use it.

!!! info "MDx settings"
    Once MDx is activated, the entry to MDx settings will be displayed in the sidebar. If you do not see the entry, please check your permission.

## Update

MDx is compatible with WordPress update. WordPress will issue a reminder in the admin panel when the updated is available. You only need to follow the instruction to complete the update.

You can also upgrade MDx manually. Just download the latest version of the theme and decompress it to overwrite old theme files.

When updating, MDx will automatically migrate all MDx-related settings. In most cases, your MDx settings will not be lost.

!!! tip "Modify the theme"
    All your changes will be lost after updating the theme. To keep your changes, please consider using [Child Themes](https://developer.wordpress.org/themes/advanced-topics/child-themes/).

!!! danger "Backup your database"
    We always recommend that you should backup your database before important operations such as updates to prevent accidental data loss. Not only updating MDx, but also WordPress updates.

## Uninstall

You only need to delete MDx in WordPress admin panel uninstall. Your MDx settings will remain in the database but will not be removed. These settings will be automatically applied the next time MDx is installed.

!!! tip "Clean MDx settings"
    All MDx data is stored in the `wp-options` table in the WordPress database. You can delete all the key values with the beginning of "mdx-" in this table.
