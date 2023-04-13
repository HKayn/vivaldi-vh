# Roadmap

This document contains all information regarding future changes and known issues on Vivaldi VH.

## Planned Features

The following will be added to Vivaldi VH in the future, in no particular order:

- Allow activation of Vivaldi VH when "Show Title Bar" is unchecked.
- [Panel at full height behind a Command Chain Flag](./command-chain-flags.md#coming-soon-panel-at-full-height).
- Allow activation of Vivaldi VH when "Show Address Bar" is unchecked.
- A "Zen Mode" where the webpage takes up the entire browser window, with the Pillar and panel floating in from the sides on demand
- One-time-use JS modification that adds all available Command Chain Flags as Command Chains.
- Ongoing updates to maintain compatibility with the latest stable Version of Vivaldi Browser.

## Considerations

The following are being considered to be added to Vivaldi VH, but have blockers that need to be resolved first:

- Allow activation of Vivaldi VH when "Show Tab Bar" is unchecked. The Pillar will be constructed using the panel instead. When the tab bar is not shown, setting panels to be non-floating will be mandated for Vivaldi VH to be active. Since this introduces an additional mandated setting, this will be behind a Command Chain Flag and disabled by default.
  - How should Vivaldi VH behave when the panel is closed? Gaps in the pillar cause erroneous behaviour across the board, and disabling Vivaldi VH entirely whenver a panel is closed would make for a jarring experience. Assume that there is no tab bar.

I appreciate any opinions that might help solve the listed issues!

## Requesting new features

When developing Vivaldi VH, I try to hold myself to these values, listed in order of importance. Please keep these in mind when requesting changes or new features.

1. Keep Vivaldi VH a CSS only modification to simplify its installation and to increase compatibility with other CSS and JS modifications. Accompanying scripts may be made available for convenience purposes only.
2. Only mandate specific browser settings when Vivaldi VH would break horribly or miss crucial functionality without them.
3. Do not restrict granular customization, e.g. do not hardcode the position of specific toolbar elements.
4. Stay as close as possible to the default properties of UI elements. Only change how things look when there are special conditions that need to be visually communicated.

## Known Issues

- When `addressbar-extend-on-focus` or `searchfield-extend-on-focus` is enabled, extending the respective field will squeeze the Pillar if the tab bar and/or the panel don't use the entire available width within the Pillar.
- Loading a webpage may stretch the Pillar if it contains an address field that's narrower than approx. `254px`.
- Toolbar components cannot be removed by dragging them to the area between the toolbar and toolbar editor window.
- Toolbar component styling is partly applied to demo toolbars inside the toolbar editor window.
