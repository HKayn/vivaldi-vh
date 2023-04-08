# Roadmap

This document contains all information regarding future fixes or changes to Vivaldi VH.

## Planned Features

The following will be added to Vivaldi VH in the future:

- One-time-use JS modification that adds all available Command Chain Flags as Command Chains
- [Panel at full height behind a Command Chain Flag](./command-chain-flags.md#coming-soon-panel-at-full-height)
- Allow activation of Vivaldi VH when "Show Address Bar" is unchecked
- Ongoing updates to maintain compatibility with the latest stable Version of Vivaldi Browser

## Considerations

The following are being considered to be added to Vivaldi VH, but have issues that need to be resolved first:

- Allow activation of Vivaldi VH when "Show Tab Bar" is unchecked. The Pillar will be constructed using the panel instead.
  - A closed or floating panel will leave a gap in the Pillar. It is unclear if Vivaldi VH should be permitted to stay activated in such a case.

I appreciate any opinions that might help solve the listed issues!

## Requesting new features

When developing Vivaldi VH, I try to hold myself to these values, listed in order of importance. Please keep these in mind when requesting changes or new features.

1. Keep Vivaldi VH a CSS only modification to simplify its installation and to increase compatibility with other CSS and JS modifications. Accompanying scripts may be made available for convenience purposes only.
2. Only mandate specific browser settings when Vivaldi VH would break horribly or miss crucial functionality without them.
3. Do not restrict granular customization, e.g. do not hardcode the position of specific toolbar elements.

## Known Issues

- When `addressbar-extend-on-focus` or `searchfield-extend-on-focus` is enabled, extending the respective field will squeeze the Pillar if the tab bar and/or the panel don't use the entire available width within the Pillar.
- Loading a webpage may stretch the Pillar if it contains an address field that's narrower than approx. `254px`.
- Toolbar components cannot be removed by dragging them to the area between the toolbar and toolbar editor window.
