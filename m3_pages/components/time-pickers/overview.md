# Time pickers

Source: https://m3.material.io/components/time-pickers/overview

- Time pickers are modal and cover the main content
- Two variants: 

  dial and 

  input
- People can select hours, minutes, or periods of time
- Make sure time can easily be selected by hand on a mobile device

![Dial time picker dial and input time picker.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmcyz4dh2-01.png?alt=media&token=726495da-d131-42f3-a766-cd787c29a235)

1. Time picker dial
2. Time picker input

## Availability & resources

| Type | Resource | Status |
| --- | --- | --- |
| Design |
| --- |
| [Design Kit (Figma)](https://www.figma.com/community/file/1035203688168086460) | Available |
| Implementation |
| --- |
| [Flutter](https://api.flutter.dev/flutter/material/TimePickerDialog-class.html) | Available |
| [android Jetpack Compose](https://developer.android.com/develop/ui/compose/components/time-pickers) | Available |
| [android MDC-Android](https://github.com/material-components/material-components-android/blob/master/docs/components/TimePicker.md) | Available |
| Web | Unavailable |

## Differences from M2

- Color: New color mappings and compatibility with 

  dynamic color

![Time picker’s old color mappings. The selected hour of 7 and AM text is purple, on a purple background.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmcz00a3d-02.png?alt=media&token=195f2e65-d46e-466a-b952-e7cfa9761d48)

M2: Time pickers had different color mappings

![Time picker's new color mappings. The selected hour of 7 and AM text is black, with different background colors.](https://firebasestorage.googleapis.com/v0/b/design-spec/o/projects%2Fgoogle-material-3%2Fimages%2Fmcz04x96-03.png?alt=media&token=a2f4ba54-7a25-4967-b3d9-bb113e40713e)

M3: Time pickers have new color mappings compatible with dynamic color
