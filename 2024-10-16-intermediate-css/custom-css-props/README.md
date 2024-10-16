# Custom Properties (Variables) Defined at the Root

- Custom properties like --primary-bg-color, --secondary-bg-color, --spacing, --border-radius, and --text-color are defined in the :root selector, which makes them available globally.
- You can easily change the values of these variables, and they will be reflected throughout the entire CSS file.

Example: --primary-font-size: clamp(1rem, 2vw, 1.5rem); controls the responsive font size, which can be reused in multiple sections.

## Reusability and Flexibility

- The custom properties make it easy to adjust the design with minimal changes. For instance, changing --primary-bg-color will automatically update the background color for the header and footer.
- --spacing is used consistently for padding and margins, which makes it easy to change the spacing across the entire site by adjusting one variable.

## Using Variables with CSS Functions:

- We’ve combined variables with functions like calc(), min(), max(), and clamp() for maximum flexibility. For example, calc(var(--spacing) / 4) dynamically calculates padding based on the --spacing value.
- Variables are used within responsive grid layouts (e.g., grid-template-columns: repeat(auto-fit, minmax(min(250px, 100%), 1fr));).

## Benefits of Using CSS Variables with Functions

- Maintainability: CSS variables reduce duplication and make it easy to change a value (like colors, sizes, or spacing) across your entire stylesheet.
- Flexibility: Combining custom properties with CSS functions such as clamp(), calc(), min(), and max() allows for responsive, dynamic layouts that adapt to different screen sizes.
- Readability: The CSS becomes more readable and easier to manage, especially in larger projects where multiple values (like colors, fonts, and spacings) are reused in various components.

## How to Test

- Try modifying the values of the custom properties (like --primary-bg-color or --spacing) to see how it affects the overall design.
- Resize the browser window to see how the clamp(), min(), and max() functions adjust the layout and typography.
