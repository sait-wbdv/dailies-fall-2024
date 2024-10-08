Explanation:
HTML Structure:

The input element (<input type="checkbox" id="menu-toggle">) is used as a checkbox that acts as a trigger for showing and hiding the mobile menu.
The label element (<label for="menu-toggle">) is used as the hamburger menu icon (☰). Clicking this label checks or unchecks the checkbox, which controls the visibility of the mobile menu.
CSS:

Inline-Block Navigation: On larger screens, the navigation items are aligned horizontally using display: inline-block on the .nav-list li elements.
Mobile Menu Toggle: The checkbox (#menu-toggle) is hidden with display: none, and the label (menu icon) is shown on smaller screens (max-width: 768px). When the checkbox is checked, the mobile menu becomes visible using the #menu-toggle:checked ~ .mobile-nav-list CSS rule.
Responsive Design: On mobile devices (below 768px width), the horizontal navigation is hidden (nav ul), and the mobile navigation menu is initially hidden with display: none. When the checkbox is checked, the mobile navigation (.mobile-nav-list) is displayed.
How It Works:
On Large Screens: The navigation bar is displayed horizontally using inline-block for the menu items.
On Small Screens: The horizontal navigation is hidden, and the hamburger menu icon (☰) appears. When the user clicks the icon, the checkbox is checked, and this triggers the mobile navigation to appear.
No JavaScript Needed: The checkbox state is used to control the display of the mobile navigation menu, so no JavaScript is required for toggling the menu.
This technique works well for simple navigation bars and is entirely CSS-driven, making it lightweight and efficient!