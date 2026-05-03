# Top app bar

Source: https://m3.material.io/components/app-bars/xr

App bars are placed at the top of the screen to help people navigate through a product

star

Note:

This is a rapidly changing space. Guidelines are primarily intended for designers at this time. Find what’s implemented in code in the [design kit](https://www.figma.com/community/file/1035203688168086460).

Extended reality (XR) interfaces have special design requirements, like showing apps in 3D space. Material has an XR-specific app bar with custom specs and guidance. See [XR developer documentation](https://developer.android.com/design/ui/xr/guides/foundations) for more details.

## Types & configurations

There is one app bar orbiter. It closely aligns with the small app bar. It can be configured to be center-aligned or left-aligned.

![Center and left-aligned app bar orbiters.](https://lh3.googleusercontent.com/PYHwyx3K5m9cJiev6I-MKCs6A60Tc5AZcpBzBcqqGQLSQMnOmNCuR1s8uzfsiZI_Yh3_LoLN1rFIo5dUEv89LWBnr3n7Qobo3yHChEb5_MJK_A=s0)

1. Center-aligned app bar
2. Left-aligned app bar

## Anatomy

![Diagrams of app bar orbiters identifying 4 internal elements.](https://lh3.googleusercontent.com/O1YVMPmvL54Qi15A17QmKNzQhv18CgDcmtGdGFtfK60IHEQNqSPp3BAdAJjZugpdBhS_ZoF3t3xcuyZcTP9McxR1FEaLkkluyBbkYPRVDnLduQ=s0)

1. Container
2. Headline
3. Trailing icons
4. Leading icon

## Color & elevation

XR uses color to communicate the elevation of UI elements and orbiters. With [spatial elevation](https://developer.android.com/design/ui/xr/guides/spatial-ui#spatial-elevation), the app bar displays above the spatial panel on the Z-axis. Elevated app bars can use any of these color options:

![3 versions of app bar elevation color strategy.](https://lh3.googleusercontent.com/7PoV7x7SsxMju6tTGEHlmT5PdcZ8VVSnzTFYcEIZlLBeIUXbp9RB9T0zphIoaYJFyzQfZyOa2AOpYIANWae0FLpDv1_lqMawI9R0TgXvjcA5=w40)![3 versions of app bar elevation color strategy.](https://lh3.googleusercontent.com/7PoV7x7SsxMju6tTGEHlmT5PdcZ8VVSnzTFYcEIZlLBeIUXbp9RB9T0zphIoaYJFyzQfZyOa2AOpYIANWae0FLpDv1_lqMawI9R0TgXvjcA5=s0)

1. Surface container
2. Surface container high
3. Surface container highest

## Measurements

![Diagrams with measurements and padding for app bar orbiters.](https://lh3.googleusercontent.com/_ROPguXE9EGmEjUSfBAPGksGu_cWhxmyKG7GLSG_qlgGQIpuD8cgrumMEgAPKdaXuxLWFZOqfUEnu6WAqapCHjBPbx1ytlUpSG7_nD0LgA2Z=w40)

Measurements and padding for app bar orbiters

## Usage

An app bar can appear in an orbiter for a more immersive experience. Currently, this spatial capability is only available in full space. In home space, use a regular app bar on the same plane as the body content to mimic a 2D experience.

An app bar’s behavior and placement changes from a 2D to a 3D experience

## Behavior

### Global context

When placed in global context, the orbiter is centered at the top of the app it controls.

It stays anchored to the app during layout or content changes.

This ensures navigation elements are always easy to find and use.

Global app bar orbiters should be centered and anchored to the top of the app

### Local context

When placed in local context, the orbiter is centered at the top of the spatial panel it controls.

It repositions in response to layout or content changes.

exclamation Caution 

Local app bar orbiters should be centered and anchored to the top of the panel. However, this is less common, so make sure that it contains actions that only affect its anchored panel.

### Additional app bars

In most cases, apps should only have one app bar orbiter, placed in global context.

exclamation Caution 

Limit the use of multiple app bars to rare cases when additional spatialization improves usability

## Placement

### Offset and inset positioning

![App bar orbiter with offset positioning.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmagu63wr-01-do.png?alt=media&token=6ea69c41-408e-4447-9022-00afd977765b)

**Do:** 

Include a 20dp margin. This visually separates the app bar orbiter from the spatial panel, and prevents content obstruction.

![App bar orbiter with inset positioning.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmagu6wj2-01-dont.jpg?alt=media&token=98bc178f-4bd0-4f16-b054-f3d4d1a15771)

**Don't:** 

Don’t overlap the app bar orbiter and spatial panel

### Horizontal alignment

![An app bar orbiter placed within the bounds of its spatial panel.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmagu80gp-02-do.png?alt=media&token=72fa7f6a-68a6-4e8f-97f9-7b8f8e35cd8f)

**Do:** 

Always align the app bar orbiter within the bounds of nearby spatial panels

![An app bar orbiter that extends beyond the width of its spatial panel.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmagu91ed-02-dont.png?alt=media&token=4c8684ea-2bac-47bf-a409-8dc87db814ce)

**Don't:** 

The app bar orbiter shouldn’t exceed the width of adjacent spatial panels

### Spatial panel alignment

By default, app bar orbiters are center-aligned to the spatial panel. Their width and placement can be adjusted to accommodate specific user needs, such as improved ergonomics or right-to-left (RTL) languages.

App bar orbiters can align to the center, left, or right of the spatial panel

### Width boundaries

An app bar orbiter’s width should adjust to stay in a person’s [field of view](https://developer.android.com/design/ui/xr/guides/spatial-ui#where-place).

This makes crucial navigation elements easy to find.

![An app bar orbiter with a width that fits in a person’s field of view.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmaguc0nf-01-do.png?alt=media&token=fd37ce05-82c0-4b99-8edf-2f0fda94034b)

**Do:** 

Adjust the width of the app bar orbiter to fit in a person’s field of view

It’s not recommended to increase the width of an app bar orbiter beyond a person’s natural [field of view](https://developer.android.com/design/ui/xr/guides/spatial-ui#where-place).

This creates a visual imbalance and makes it difficult to find navigation elements.

![An app bar orbiter that exceeds the panel’s width and a person’s field of view.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmagv5qxq-02-dont.png?alt=media&token=30b6f21c-4aa4-4768-92ac-014e1dded8a1)

**Don't:** 

Avoid expanding the app bar orbiter beyond the adjacent panel’s width and a person’s field of view

### Adaptable width

When placed in a local context, an app bar orbiter can expand to the width of its adjacent spatial panel.

Be sure the orbiter stays in a person’s field of view, and test for usability.

exclamation Caution 

Use caution before expanding the app bar’s width to match its spatial panel. The orbiter may not fit in a person’s primary field of view.

## Accessibility considerations

[XR accessibility](https://developer.android.com/design/ui/xr/guides/get-started#make-app) guidelines are still evolving. XR app bars should follow applicable Material [app bar accessibility standards](./accessibility.md).
