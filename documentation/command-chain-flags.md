# Command Chain Flags

Vivaldi VH contains several changes to the UI of Vivaldi Browser besides the Pillar layout. Not everyone might prefer to have all of these changes applied. Command Chain Flags allow you to control these features of Vivaldi VH right inside the Vivaldi Browser, without modifying any CSS code.

## Setup Guide

You can set up Command Chain Flags for specific features by following the steps below.

1. [Create a Command Chain](https://help.vivaldi.com/desktop/shortcuts/command-chains/#Create_a_Command_Chain) in the Quick Commands settings of Vivaldi Browser.
2. Give this command chain a name that matches the flag you would like to apply, for example `vvh-disable-addressfield-extend-on-focus`.
3. [Open the Toolbar Editor](https://help.vivaldi.com/desktop/appearance-customization/edit-toolbars/#Customize_toolbars) and select "Command Chains" from the dropdown. Grab your created Command Chain and drag it into one of your toolbars.

## Available Flags

### Grow width of address bar components to occupy free space

*Enabled by default.*

To disable: `vvh-disable-addressbar-universal-flex-grow`

Individual components in the address bar are distributed evenly across the width of each row. If the title bar is shown, this can also grow their click area.

Additionally, flexible spacers inside the address bar are hidden.

### Grow width of status bar components to occupy free space

*Enabled by default.*

To disable: `vvh-disable-statusbar-universal-flex-grow`

Individual components in the status bar are distributed evenly across the width of each row. This can also grow their click area.

Additionally, flexible spacers inside the status bar are hidden.

### Permanent padding around webpage

*Enabled by default.*

To disable: `vvh-disable-webpage-permanent-padding`

The padding around webpages that normally only appears when tab tiling is active is permanently visible.

**Note:**: This feature is not available on Vivaldi VH VivalArc Edition.

### Extend address field width when editing input

*Enabled by default.*

To disable: `vvh-disable-addressfield-extend-on-focus`

The address field extends beyond the Pillar width when the input area is in focus.

### Extend search field width when editing input

*Disabled by default.*

To enable: `vvh-enable-searchfield-extend-on-focus`

The search field extends beyond the Pillar width when the input area is in focus.

### Invert position of hidden extensions toggle

*Disabled by default.*

To enable: `vvh-enable-extensions-invert-toggle-position`

The button that toggles the visibility of hidden extensions is placed to the other side of the extensions grid.

### Incorporate panel into Pillar

*Disabled by default.*

To enable: `vvh-enable-panel-in-pillar`

When the panel is on the same side as the tab bar, it is incorporated into the Pillar between the window edge and the tab bar.

### Title bar at full width

*Disabled by default.*

To enable: `vvh-enable-titlebar-full-width`

When the title bar is enabled, it takes up the entire width of the browser window.

**Note:**: On Vivaldi VH VivalArc Edition, this feature is permanently enabled and cannot be disabled.

## Precedence Rules

It is currently possible to have flags set that `enable` and `disable` the same feature at the same time. Additionally, each feature has a default state according to what I think is the best default experience for Vivaldi VH.

For each flag, the following precedence rules apply:

1. The `disable` flag always disables a feature.
2. The `enable` flag enables a feature if the `disable` flag is not set.
3. The default state of a feature applies if neither flag is set.
