# Explanation of CSS Functions

## calc(): Combines different units to create flexible layouts

Example: width: calc(100% - 20px); can adjust the element's width based on both percentage and fixed units.

## min(): Ensures the element doesn’t shrink below a certain size

Example: width: min(90%, 600px); means the width is either 90% of the viewport or 600px, whichever is smaller.

## max(): Ensures the element does not exceed a certain size

Example: minmax(min(250px, 100%), 1fr); ensures each gallery item is at least 250px or 100% of the available space, but no larger than 1 fraction of the available grid space.

## clamp(): Sets a responsive range for properties like font sizes or padding

Example: font-size: clamp(1rem, 2vw, 1.5rem); sets the font size to a minimum of 1rem, adjusts according to the viewport (2vw), and limits it to a maximum of 1.5rem.
