# Elevation

Source: https://m3.material.io/styles/elevation/tokens

Elevation is the distance between two surfaces on the z-axis

## Tokens

Elevation levels can be implemented with tokens. Surface tint color is deprecated. Use elevation level tokens (0–5) instead. [Learn more about design tokens](../../m3/pages/design-tokens/overview)

Elevation arrow\_drop\_down

search

view\_list

Default, Light arrow\_drop\_down

#6750A4  Surface tint color

+5

+4

+3

+2

+1

0

## Component elevation

Most components have a default elevation. Component elevation is only used to determine where the component sits in relation to other components, including when hovered or focused (which usually raises elevation by one level). Elevation has no shadow or value of its own by default.

| Resting level | Component | DP Height |
| --- | --- | --- |
| 5 | (not assigned as resting level) | 12dp |
| 4 | (not assigned as resting level) | 8dp |
| 3 | Date pickers  Dialogs (modal)  Extended FAB  FAB  FAB menu (close button)  Search  Time pickers | 6dp |
| 2 | App bar (scrolled)  Menu  Navigation bar  Rich tooltip  Toolbar | 3dp |
| 1 | Banner  Bottom sheet (modal)  Button (elevated)  Card (elevated)  Chips (elevated)  Navigation drawer (modal)  Side sheet (modal) | 1dp |
| 0 | App bar (not scrolled)  Buttons (filled, tonal, outlined)  Button groups  Cards (filled, outlined)  Carousel  Chips  Dialog (full-screen)  Extended FAB (in navigation rail)  FAB (in navigation rail)  FAB menu (list items)  Icon buttons  List  Navigation rail  Segmented button  Side sheet (docked)  Slider  Split button  Tabs | 0dp |
