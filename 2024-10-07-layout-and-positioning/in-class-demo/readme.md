Explanation for Students:
Static Position (Default):

By default, all elements are position: static. They appear in the normal document flow without any special positioning.
css
Copy code
.static-box {
    /* No position property needed, static is default */
}
Relative Position:

The element is positioned relative to its normal position. We can move it from its original spot using top, left, right, and bottom.
css
Copy code
.relative-box {
    position: relative;
    top: 20px;  /* Moves 20px down from its normal position */
    left: 10px; /* Moves 10px right from its normal position */
}
Absolute Position:

The element is positioned relative to its nearest positioned ancestor. If no ancestor is positioned, it will be positioned relative to the viewport. In this case, we put the .absolute-box inside a container (.relative-wrapper) that has position: relative, so the absolutely positioned box will be placed relative to that.
css
Copy code
.relative-wrapper {
    position: relative;
}

.absolute-box {
    position: absolute;
    top: 20px;  /* 20px down from the top of the .relative-wrapper */
    right: 20px; /* 20px from the right edge of the .relative-wrapper */
}
Fixed Position:

The element is positioned relative to the viewport. It remains fixed in place even when the page is scrolled. This is useful for creating elements like sticky headers or floating menus.
css
Copy code
.fixed-box {
    position: fixed;
    top: 20px;  /* Stays 20px from the top of the viewport */
    right: 20px; /* Stays 20px from the right side of the viewport */
}
Sticky Position:

The element behaves like relative until you scroll past a certain point. After that, it behaves like fixed and sticks to the top of the viewport (in this case, top: 0).
css
Copy code
.sticky-box {
    position: sticky;
    top: 0;  /* Sticks to the top of the viewport when scrolled */
}
Live Coding:
Start by showing them the static example (default behavior).
Move on to relative and explain how it offsets from the normal position.
For absolute, show how it's positioned within a container (using the .relative-wrapper).
Scroll down and explain how the fixed element stays in place while the rest of the content moves.
Finally, demonstrate how the sticky element becomes fixed after scrolling past it