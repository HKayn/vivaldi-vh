# Roadmap

This document contains all information regarding future changes and known issues on Vivaldi VH.

## Planned Features

The following will be added to Vivaldi VH in the future, in no particular order:

- A "Zen Mode" where the webpage takes up the entire browser window, with the Pillar and panel floating in from the sides on demand.
- One-time-use JS modification that adds all available Command Chain Flags as Command Chains.
- Ongoing updates to maintain compatibility with the latest stable version of Vivaldi Browser.

## Considerations

The following are being considered to be added to Vivaldi VH, but have blockers that need to be resolved first:

- None at the moment!

## Requesting new features

When developing Vivaldi VH, I try to hold myself to these values, listed in order of importance. Please keep these in mind when requesting changes or new features.

1. Keep Vivaldi VH a CSS only modification to simplify its installation and to increase compatibility with other CSS and JS modifications. Accompanying scripts may be made available for convenience purposes only.
2. Only mandate specific browser settings when Vivaldi VH would break horribly or miss crucial functionality without them.
3. Do not restrict granular customization, e.g. do not hardcode the position of specific toolbar components.
4. Stay as close as possible to the default properties of UI elements. Only change how things look when there are special conditions that need to be visually communicated.

## Known Issues

- When `addressbar-extend-on-focus` or `searchfield-extend-on-focus` is enabled, extending the respective field will squeeze the Pillar if the tab bar and/or the panel don't use the entire available width within the Pillar.
- Loading a webpage may stretch the Pillar if it contains an address field that's narrower than approx. `254px`.
- Toolbar components cannot be removed by dragging them to the area between the toolbar and toolbar editor window.
- Toolbar component styling is partly applied to demo toolbars inside the toolbar editor window.
- When the panel does not touch the left or right window edge, panel resizing will behave in unexpected ways, but still be fully functional.
- When the panel does not touch the left or right window edge, the "Add Web Panel" popup will be slightly misplaced, but still fully functional.
- Vivaldi VH activation toggles do not fully replace the original command chain icon inside the toolbar editor window. This does not occur once the toggle is placed inside a toolbar.
