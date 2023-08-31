# Changelog

## v1.2.2 (2023-08-31)

### Fixes

- When the title bar is disabled, the menu button in the address bar will no longer break out of its designated space.
- When the title bar is enabled, the address bar will now have the correct background.

## v1.2.1 (2023-04-20)

### Fixes

- When the title bar is not shown, Vivaldi VH will no longer reserve unnecessary space for window buttons when "Use Native Window" is enabled.
- When the title bar is not shown, toolbar components inside the address bar may grow their click area when "Use Native Window" is enabled, since the address bar no longer acts as a draggable region.

---

## v1.2.0 (2023-04-18)

### Changes

- Vivaldi VH no longer requires the title bar to be shown.
- Toolbar linebreaks are now available.
  - *"[Click here to find out how to set up toolbar linebreaks.](../command-chain-utilities.md)"*
- Command Chain Flags, Command Chain Utilities and flexible spaces are now highlighted in the toolbar editor.
- Command Chain Flags and Command Chain Utilities now remain hidden when Vivaldi VH is disabled due to invalid settings.
- When `addressbar-universal-flex-grow` or `statusbar-universal-flex-grow` is disabled, components of the respective toolbar are now initially justified to the left instead of centered.
  - *"This change was required to implement the layout of Vivaldi VH without a title bar. Rest assured that centered toolbar components can still be achieved using flexible spaces."*
- Documentation and demo images have been updated.
- Unused source code has been removed.

---

## v1.1.0 (2023-04-09)

### Changes

- The button that toggles hidden extensions is now always to the right of the extensions grid.
  - *"Before this change, the position of this button would change to always be on the window edge. It was the only element that would change its position inside the address bar or status bar when the Pillar moved from one side to the other, and that didn't feel right in hindsight. It's now permanently to the right of the extensions, just like in the default UI. For anyone who preferred it on the left side, a Command Chain Flag has been added for inverting the position."*
- Command Chain Flags for inverting the position of the hidden extensions toggle are now available.
- The logic that calculates the width of an extending input field has been improved to take additional browser settings into account.
  - *"The intention is to not cover the panel column. Since the panel can also have a visible toggle or be hidden entirely, these settings are now being taken into account when calculating how wide the address field or search field can be."*
- The title bar height and address box row height have been changed to 25px and 34px respectively.
  - *"This should more closely match the default heights of the respective bars."*
- Redudant custom properties have been removed.
- Updated documentation.

### Fixes

- The height of title bar elements will no longer change in unintended ways when changing the user interface zoom setting.
- The default browser notification will no longer disrupt the UI layout.
- Fixed a case where the webpage would gain an unintended margin on specific browser settings.
  - *"Specifically, this right margin would appear if the tab bar and the panel were on the right side with the panel toggle enabled and the panel hidden."*

---

## v1.0.0 (2023-04-08)

First release of Vivaldi VH.
