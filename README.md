# Tailwind CSS - Missing File Extensions in `content` Option

This repository demonstrates a common issue when using Tailwind CSS: the stylesheet processor fails to pick up styles from certain files because the `content` option in `tailwind.config.js` doesn't include the correct file extensions.

## Problem

The `tailwind.config.js` file incorrectly specifies the file types to scan for Tailwind directives (e.g., class names).  This can lead to the styles not being processed or applied.

## Solution

Ensure that the `content` option in `tailwind.config.js` includes all relevant file extensions.  The correct file extensions must be listed in the array for the processor to correctly identify and process Tailwind directives in your files.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Try to run your application. You should observe that some styles are missing.
4. Look at `bug.js` and `bugSolution.js` to compare the incorrect and corrected `tailwind.config.js` configuration.

## How to Fix

Update the `content` option to correctly include all relevant file extensions within your project, as shown in `bugSolution.js`.