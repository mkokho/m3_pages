# Canonical layouts

Source: https://m3.material.io/foundations/layout/canonical-layouts/list-detail

Canonical layouts are designs for common screen layouts across all window size classes

Many layouts can be established based on the relationship of a list and a detail view.

Key use cases for this layout include parent-child pairings of information like:

- Text message + conversation
- File browser + open folder
- Musical artist + album detail
- Settings + category detail
- Email inbox + selected email

![An email app in a list-detail layout in a medium window size.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxye03l6-1.png?alt=media&token=2e8b59dc-2e41-4147-9fe0-640a4e04651f)

1. List
2. Detail

## Usage

Use the list-detail view for displaying browsable content and quickly showing details.  
  
Examples include: showing a series of conversations and a text message; browsing files and seeing their details; or browsing multiple albums and seeing individual track information in an adjacent view.

![Several stacked cards make up the list area on the left pane, while the detail area is a single section on the right pane.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxye1vad-2.png?alt=media&token=aee278d7-9838-4779-b585-9646dbd4f5f9)

Simplified diagram of:

1. List area
2. Detail area

## Dividing space

![Compact windows have 1 pane, while medium and expanded windows can have 2 panes for list-detailed views.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxye2xeh-3.png?alt=media&token=4b687afc-aa4b-4802-825b-5bee568e0801)

The most basic list-detail views for compact, medium, and expanded layouts

A list-detail view uses two panes: one for a list or group of items and the other for a detailed view. Depending on the window class, the two panes may appear together in the same layout or across separate layouts.  
  
List-detail canonical layouts use the same pane guidance as all single and two-pane layouts, including special behavior for foldables.

| **Window size class (dp)** | **Visible panes** |
| --- | --- |
| Compact (0-599) | 1 pane |
| Medium (600-839) | 1 (recommended) or 2 panes |
| Expanded (840+) | 2 panes |
| Large (1200-1599) | 2 panes |
| Extra-large (1600+) | 2 panes |

## Across window size classes

### Compact

- Use a single-pane layout
- Only one view is visible at a time (either list or detail)

![Single pane layout on 3 devices with compact window sizes.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxye4k9e-4.png?alt=media&token=27b207c4-e0fd-4fec-83f7-cf0742d7451c)

1. Phone in portrait orientation
2. Closed foldable
3. Tablet in split-screen mode

### Medium

- Use a single-pane layout for information-dense content or longer interactions

![Single-pane layout on a foldable open flat and a tablet in portrait orientation.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxygqujc-5.png?alt=media&token=18a4bae5-6e67-4b37-bfff-85c49507e298)

1. Foldable open flat
2. Tablet in portrait orientation

1. Use a two-pane layout for information-dense content, or quicker interactions
2. To avoid cramped pane widths, use a bottom navigation bar or modal navigation drawer with two-pane layouts in medium only

![Two-pane layout on a foldable open flat and a tablet in portrait orientation.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxygruxu-6.png?alt=media&token=d4c8f911-ecc1-4c60-850d-1c45ab780c65)

1. Foldable open flat
2. Tablet in portrait orientation

### Expanded, large, and extra-large

- Use a two-pane layout

![Two-pane layout on a phone and tablet, both in landscape orientation.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxygtbb1-7.png?alt=media&token=2dafae6a-5fa5-4ec4-a25c-3cbd582dd62a)

1. Phone in landscape orientation
2. Tablet in landscape orientation

## Behavior

### Single vs two-pane

- Back button: Appears in detail view only for single-pane layouts
- Selected state: Appears only in list view for two-pane layouts
- Visual focus: Use [explicit and implicit grouping](../understanding-layout/spacing.md#efb4667d-f942-4019-8cd8-1fcb366e392d) to direct focus in two-pane layouts

![A two-pane layout shows the selected list item, while a single pane layout uses a Back button to return to the list.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Flxygv3fn-8.png?alt=media&token=c7e6d4e6-dfdc-4075-81b1-95517c08f3b6)

Navigating between list and detail views is different in each layout

### Transitioning between layouts

The amount of available space is dynamic and changes based on user behavior, such as rotating or unfolding a device, or entering a multi-window mode.

A two-pane list-detail layout adapts to a one-pane layout when the device is rotated, changing from expanded to medium window class

#### No selected list item

The single-pane screen shows the list, and the two-pane screen shows placeholder content in the detail pane.

In some use cases, such as multi-select, the pane last interacted with should remain visible when switching back to single-pane view.

If no item in the list view is selected when a foldable is opened, the revealed pane displays an empty detail view

**Selected list item**

When going from a single- to two-pane view, both panes should be shown. The selected item’s details are visible.

When going from a two- to single-pane view, the result depends on the product behavior:

- Generally, the detail pane should be shown on the single-pane view, and an app bar appears.
- However, if the product supports selected list items without navigating deeper, like multi-select, it can show the list view instead with the item selected.
- The most important rule is consistency. If the single pane showed the list view before, it should revert to the list view when going back to a single pane.

If an item in the list is selected when a foldable is opened, the revealed pane displays that item’s detail view

If an item in the list is selected when a foldable is closed, the list view is hidden and the detail view is shown in the single pane

If no list item is selected, list pane remains visible and detail pane hides.  
  
In some use cases, such as multi-select, the pane last interacted with should remain visible.

If no item in the list is selected when a foldable is closed, the detail view is hidden and the list view is shown in the single pane

In most cases, a state should be saved when navigating between detail views. Detail views with read and unread content fall into this use case.

The scroll position of a detail view is retained even after navigating to other list items
