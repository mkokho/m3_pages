# Loading indicator

Source: https://m3.material.io/components/loading-indicator/overview

Loading indicators show the progress for a short wait time

- Recommended as a replacement for indeterminate 

  circular progress indicators
- Always reflect an ongoing process and are never simply decorative
- Used for pull-to-refresh interactions
- Not used for processes that transition from indeterminate to determinate
- Capture attention through motion

1. Loading indicator
2. Contained loading indicator

## Availability & resources

| Type | Resource | Status |
| --- | --- | --- |
| Design |
| --- |
| [Design Kit (Figma)](https://www.figma.com/community/file/1035203688168086460) | Available |
| Implementation |
| --- |
| [android Jetpack Compose: Expressive](https://developer.android.com/reference/kotlin/androidx/compose/material3/package-summary#LoadingIndicator(androidx.compose.ui.Modifier,androidx.compose.ui.graphics.Color,kotlin.collections.List)) | Available |
| [android MDC-Android: Expressive](https://github.com/material-components/material-components-android/blob/master/docs/components/LoadingIndicator.md) | Available |
| Web: Expressive | Unavailable |

## M3 Expressive update

**May 2025**

The loading indicator is designed to show progress that loads in under five seconds. It should replace most uses of the indeterminate circular progress indicator. [More on M3 Expressive](https://m3.material.io/blog/building-with-m3-expressive)

New component added to catalog.

Loading indicators:

- Are used in pull-to-refresh functionality
- Can be contained or uncontained
- Use shape and motion to capture attention
- Can scale in size

Loading indicators are used in the pull-to-refresh behavior
