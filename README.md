# React Native Dimensions.get() returns undefined

This repository demonstrates a common issue in React Native applications where `Dimensions.get('window')` or `Dimensions.get('screen')` returns `undefined`. This typically happens when these functions are called before the layout has been fully measured, often leading to unexpected behavior or crashes.

The `DimensionsBug.js` file showcases the problematic code, while `DimensionsBugSolution.js` provides a solution to address the issue.  The solution involves using the `useEffect` hook with the `LayoutAnimation` API for a smooth UI update, ensuring the dimensions are available before usage.