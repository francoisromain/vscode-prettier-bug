# VS Code / Prettier plugin / bug

related issue: https://github.com/prettier/prettier-vscode/issues/1425

In `index.ts`, there is a trailing coma added on save at the end of line 4. Nothing in the project config requires this coma.

If I disable the CS Code prettier plugin and save the file again, the coma is removed (which is what we want).

This bug occurs since the plugin updated to version 5.0.0.
