# Expo Image Component: Incorrect URI format for local images

This repository demonstrates a common error when using the Expo `Image` component with local image URIs. The error arises from an incorrectly formatted URI, causing the image to fail to render.

## Bug Description

The `Image` component in Expo fails to display local images when the URI provided to the `source` prop does not adhere to the correct `file://` scheme and full file path format.

## Reproduction Steps

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run the app using Expo Go or a similar Expo client.
4. Observe that the image in `bug.js` fails to render.
5. Compare it with the correctly implemented version in `bugSolution.js` which successfully renders the image.

## Solution

The solution involves ensuring the URI provided to the `source` prop follows the `file:///path/to/your/image.jpg` format, including the `file://` scheme and the full path to the image file.