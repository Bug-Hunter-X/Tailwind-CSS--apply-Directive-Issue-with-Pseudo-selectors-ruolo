# Tailwind CSS @apply Directive Issue with Pseudo-selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to correctly apply styles when used with pseudo-selectors like `:hover` or `:focus` within a class.

## Bug Description

The `@apply` directive, intended for applying pre-defined utility classes, does not correctly handle pseudo-selectors.  This can lead to unexpected styling behaviour, particularly with interactive elements.

## Reproduction

1. Clone this repository.
2. Open `bug.css` to see the incorrect implementation.
3. Observe the lack of hover effect on the button.
4. Open `bugSolution.css` to see the corrected approach.  

## Solution

The solution involves applying pseudo-selector classes directly within the element's style rather than using the `@apply` directive.

This issue highlights a limitation of using `@apply` with pseudo-selectors. The best practice is to apply these styles directly in the HTML.  This avoids unexpected behaviour.