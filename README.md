# React Native FlatList Performance Issue: Incorrect Key Extraction

This repository demonstrates a common performance issue in React Native's `FlatList` component when dealing with large datasets.  The problem arises from an incorrectly implemented `keyExtractor` function, which leads to inefficient rendering and potential performance bottlenecks.

The `FlatListBug.js` file showcases the problematic code, while `FlatListBugSolution.js` provides the corrected implementation.

## Problem
Incorrectly providing keys to the `FlatList` can lead to slow rendering, increased memory usage, and ultimately crashes in some cases. This is because React Native's diffing algorithm relies on keys for efficient updates.