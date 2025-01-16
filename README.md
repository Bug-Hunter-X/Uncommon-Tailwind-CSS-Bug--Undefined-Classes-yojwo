# Uncommon Tailwind CSS Bug: Undefined Classes

This repository demonstrates a common yet easily overlooked error in Tailwind CSS: using undefined classes.  This can occur due to typos, outdated configuration, or inconsistencies between your CSS and Tailwind's configuration.

## Bug Description
The `bug.js` file contains JavaScript code that attempts to use a Tailwind CSS class that isn't defined in the `tailwind.config.js` file.  This results in the class having no effect, or in some cases, causing rendering issues or errors.

## Solution
The `bugSolution.js` file provides a corrected version. The solution involves ensuring that all Tailwind CSS classes used are correctly defined and included in the configuration file, or using PurgeCSS to remove unused classes from the final CSS output.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` (if necessary).
3. Observe the outcome of running `bug.js` versus `bugSolution.js`. You'll notice the difference in how the class is handled and its effect on the output.

## Lessons Learned
Always double-check your Tailwind CSS class names against your `tailwind.config.js` file. Use a linter or a similar tool to check for these types of errors before deployment. Ensure that your config file is up to date and properly configured.