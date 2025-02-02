# Tailwind CSS: Missing Classes Bug

This repository demonstrates a bug where Tailwind CSS classes are not applied correctly due to issues with class purging or class inclusion.  Custom classes defined using the `@apply` directive are missing from the generated CSS, even though the Tailwind configuration and imports appear to be set up correctly. 

## Steps to Reproduce

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the development server (e.g., using Vite or Webpack). 
4. Observe that the element with the `bg-custom-blue` class does not have the expected blue background color.

## Solution

The solution involves ensuring that the `content` option in your `tailwind.config.js` correctly includes all files where Tailwind classes are used. It's crucial to check for any typos or incorrect paths.

See `bugSolution.js` for the corrected configuration.