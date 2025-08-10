# Mobile-Friendly-Using-CSS-Media-Queries

1. What are media queries?
Media queries are CSS rules that apply styles based on conditions such as screen width, height, orientation, or resolution.
They allow you to create responsive designs that adapt to different devices.
Example:

css
Copy
Edit
@media (max-width: 768px) {
  body { background-color: lightblue; }
}
2. Explain mobile-first vs desktop-first CSS design.
Mobile-first:

Write styles for small screens first, then add media queries for larger screens using min-width.

Pros: Usually lighter for mobile, better for performance.

Desktop-first:

Write styles for large screens first, then override for smaller screens using max-width.

3. How do you test responsiveness?
Chrome DevTools Device Toolbar (Ctrl+Shift+M / Cmd+Shift+M on Mac)

Resize browser window manually

Use real devices (mobile/tablet)

Online testing tools like BrowserStack

4. What units are best for responsive layouts?
Relative units like %, em, rem, vw, vh

Avoid fixed pixel widths for layout elements

Use max-width for images and containers

5. What is viewport meta tag?
The viewport meta tag tells the browser how to control the page's dimensions and scaling on mobile devices.
Example:

html
Copy
Edit
<meta name="viewport" content="width=device-width, initial-scale=1.0">
width=device-width: matches the screen’s width

initial-scale=1.0: sets initial zoom level

6. How does flexbox help in responsive design?
Automatically adjusts the size of elements based on available space

Supports flexible alignment, wrapping, and ordering of elements

Easily switches from horizontal to vertical layout with flex-direction

7. Difference between absolute and relative units?
Absolute units: Fixed sizes (e.g., px, cm) — do not scale based on screen size

Relative units: Adjust based on parent or viewport size (e.g., %, em, rem, vw, vh) — better for responsiveness

8. How to handle images in responsive design?
Use max-width: 100%; height: auto; to make images scale

Use modern formats like WebP for faster loading

Consider <picture> element and srcset for different resolutions

9. What is adaptive vs responsive design?
Responsive Design: Fluid layout that changes continuously based on screen size using flexible grids and media queries.

Adaptive Design: Uses fixed layouts for specific breakpoints (e.g., one layout for 320px, another for 768px).

10. Explain CSS grid responsiveness.
CSS Grid allows you to create two-dimensional layouts that adjust based on screen size.

You can use grid-template-columns with fr units or auto-fit and minmax() for responsive behavior.
Example:

css
Copy
Edit
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}
