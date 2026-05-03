# Side sheets

Source: https://m3.material.io/components/side-sheets/accessibility

Side sheets show secondary content anchored to the side of the screen

## Use cases

People should be able to dismiss the side sheet using assistive technology.

## Interaction & 

Material requires that a close affordance, such as a close icon button, is always present within a side sheet.

![Side sheet correctly designed with close icon in upper right corner.](https://lh3.googleusercontent.com/0LSf0hnC19HAyDDf88fqzUUo62971bFb2XWjHguURc3jJbZpy8ejGuIyFR-2MSFM27gLA3LjupVjSj8E5kEuDJG7IqeHD17NaXUOXKsEHdP8=s0)

**Do:** 

A close icon button makes the side sheet easy to dismiss

![Side sheet incorrectly designed with no close icon button.](https://lh3.googleusercontent.com/bGugN52A6j4bvI4smHp21cQzZbZv4qaF9YBYdKZDD51XL6yAkHSY_KVtpUF7HkL6G04T2w61MQeJo-E8SqmPJx6OuO9YMeBqpjP7AOhc_yNi=s0)

**Don't:** 

Without a close icon button, people can’t predict the opening and closing flow of side sheets, or know if the sheet is transient or permanent

## Initial focus

Actions within a side sheet can be focused by tab order using a keyboard or switch control.

![Side sheet diagram showing the focus order of headline, close, save, cancel.](https://lh3.googleusercontent.com/MuS9aCeC3P_ukbbopUpL7M9rV8VhBbirg3UofV-_SA7g-v4ABLSE8zgMWQOlHo7WP5XEd7s-KyR15aPB360mGPFofc_F3uKb1Sy7iQ8iOZ0dGA=s0)

Visible focus shown on the available actions within a side sheet:

1. Headline
2. Close
3. Cancel
4. Save

## Keyboard navigation

| Keys | Actions |
| --- | --- |
| **Tab** | Focus lands on (non-disabled) icon button |
| **Space** or **Enter** | Activates the (non-disabled) icon button |

## Labeling

The accessibility role for a side sheet is **Dialog**.

![Side sheet showing the accessibility role as dialog.](https://lh3.googleusercontent.com/ogti7RlWzhZNIER0PGHxR2hM--wMncqBhexq_aLUiY6OPM1C5NeuaWV29SOOqi5gjdr7dGbCFrlPMnQ2hX5pgrWhVUrQVhUmESeeg09ZQhdB=w40)![Side sheet showing the accessibility role as dialog.](https://lh3.googleusercontent.com/ogti7RlWzhZNIER0PGHxR2hM--wMncqBhexq_aLUiY6OPM1C5NeuaWV29SOOqi5gjdr7dGbCFrlPMnQ2hX5pgrWhVUrQVhUmESeeg09ZQhdB=s0)

The role for side sheets is **Dialog**
