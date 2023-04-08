# Command Chain Flags

Vivaldi VH contains several changes to the UI of Vivaldi Browser besides the Pillar layout. Not everyone might prefer to have all of these changes applied. Command Chain Flags allow you to control these features of Vivaldi VH right inside the Vivaldi Browser, without modifying any CSS code.

## Setup Guide

You can set up Command Chain Flags for specific features by following the steps below.

1. [Create a Command Chain](https://help.vivaldi.com/desktop/shortcuts/command-chains/#Create_a_Command_Chain) in the Quick Commands settings of Vivaldi Browser.
2. Give this command chain a name that matches the flag you would like to apply, for example `vvh-disable-addressfield-extend-on-focus`.
3. [Open the Toolbar Editor](https://help.vivaldi.com/desktop/appearance-customization/edit-toolbars/#Customize_toolbars) and select "Command Chains" from the dropdown. Grab your created Command Chain and drag it into one of your toolbars.

## Precedence Rules

It is currently possible to have flags set that enable and disable the same feature at the same time. Additionally, each feature has a default state according to what I think is the best default experience for Vivaldi VH.

For each flag, the following precedence rules apply:

1. The `disable` flag always disables a feature.
2. The `enable` flag enables a feature if the `disable` flag is not set.
3. The default state of a feature applies if neither flag is set.

## Available Flags

### Extend address field width when editing input

**`vvh-enable-addressfield-extend-on-focus`** (default) \
`vvh-disable-addressfield-extend-on-focus`

The address field extends beyond the Pillar width when the input area is in focus.

### Extend search field width when editing input

**`vvh-enable-searchfield-extend-on-focus`** (default) \
`vvh-disable-searchfield-extend-on-focus`

The search field extends beyond the Pillar width when the input area is in focus.

### Permanent padding around webpage

**`vvh-enable-webpage-permanent-padding`** (default) \
`vvh-disable-webpage-permanent-padding`

The padding around webpages that normally only appears when tab tiling is active is permanently visible.

### Grow width of address bar components to occupy free space

**`vvh-enable-addressbar-universal-flex-grow`** (default) \
`vvh-disable-addressbar-universal-flex-grow`

The width of individual components in the address bar grows to occupy free space in their row. This can also grow their click area.

Additionally, flexible spacers inside the address bar are hidden.

### Grow width of status bar components to occupy free space

**`vvh-enable-statusbar-universal-flex-grow`** (default) \
`vvh-disable-statusbar-universal-flex-grow`

The width of individual components in the status bar grows to occupy free space in their row. This can also grow their click area.

Additionally, flexible spacers inside the status bar are hidden.

### *(Coming soon!)* Panel at full height

`vvh-enable-panel-full-height` \
**`vvh-disable-panel-full-height`** (default)

When the panel is on the same side as the tab bar, it is no longer incorporated into the Pillar, but instead positioned at full height between the Pillar and the webpage.
