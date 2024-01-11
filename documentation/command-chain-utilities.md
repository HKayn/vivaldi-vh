# Command Chain Utilities

Command Chain Utilities allow you to fine-tune the layout of your toolbars.

## Setup Guide

You can set up Command Chain Utilities for specific features by following the steps below.

1. [Create a Command Chain](https://help.vivaldi.com/desktop/shortcuts/command-chains/#Create_a_Command_Chain) in the Quick Commands settings of Vivaldi Browser.
2. Give this command chain a name that matches the utility you would like to use, for example `vvh-insert-linebreak`.
3. [Open the Toolbar Editor](https://help.vivaldi.com/desktop/appearance-customization/edit-toolbars/#Customize_toolbars) and select "Command Chains" from the dropdown. Grab your created Command Chain and drag it into one of your toolbars.

## Available Utilities

### Toolbar linebreak

`vvh-insert-linebreak`

When placed in a toolbar, this will move all toolbar components after it to a new row.

The name can have any suffix; names such as `vvh-insert-linebreak2` or `vvh-insert-linebreak-middle` will be recognized as toolbar linebreaks.

Special interactions:

- If a Toolbar Linebreak is placed immediately before and after a mail search toolbar component, that search bar will grow to take up the full width of the toolbar that contains it.

### Vivaldi VH activation toggle

`vvh-toggle-on` \
`vvh-toggle-off`

When placed inside a toolbar, these will receive a special icon and be shown depending on the current activation state of Vivaldi VH:

- `vvh-toggle-off` will only be shown if Vivaldi VH is currently active.
- `vvh-toggle-on` will only be shown if Vivaldi VH is currently disabled due to invalid settings.

The name can have any prefix and/or suffix; names such as `vvh-toggle-on-1` or `Turn Vivaldi VH off (vvh-toggle-off)` will be recognized as Vivaldi VH activation toggles.

**Note:** Command Chains with these names will **not** change the activation state of Vivaldi VH by themselves! Vivaldi VH enables itself depending on specific browser settings such as the tab bar position. Command Chains with these names should execute commands that change the relevant browser settings, e.g. "Tabs on Top" or "Tabs on Left".
