### Desktop design

![alt text](/solution_imgs/desktop_solution.png)

### Mobile design

![alt text](/solution_imgs/mobile_solution.png)

### Tablet design

![alt text](/solution_imgs/tablet_solution.png)

### The challenge

The challenge was to create a responsive design that would look good on both desktop and mobile devices.

### How we've solved the challenge
I used CSS Grid to create a responsive layout that would adjust to different screen sizes.

- Add CSS Grid layout with responsive breakpoints
- Create custom color variables for consistent theming
- Implement smooth transitions for width changes
- Add tablet-specific layout for better UX
- Update README with solution screenshots and learnings

### Challenges encountered

1. **Grid Layout Complexity**
   - Creating a responsive grid that accommodates differently sized cards
   - Managing the unique layout where the first card spans two columns and the last card spans two rows
   - Ensuring the grid maintains visual hierarchy across different screen sizes
   - Implementing a tablet layout that effectively breaks down the desktop design

2. **Responsive Design Issues**
   - Cards initially stacked incorrectly in mobile view due to inherited grid positions
   - Had to carefully consider breakpoints (768px for mobile, 1024px for tablet)
   - Needed to adjust the container width (90% mobile, 75% tablet, 55% desktop) for optimal viewing
   - Added max-width to prevent layout from becoming too wide on large screens

3. **CSS Specificity Challenges**
   - Encountered issues with grid positioning rules conflicting between breakpoints
   - Explored two solutions:
     ```css
     /* Solution 1: Using !important */
     .card {
         grid-column: 1 !important;
     }
     
     /* Solution 2: Using specific selectors */
     .card:nth-child(1), .card:nth-child(2)... {
         grid-column: 1;
     }
     ```
   - Learned about the trade-offs between using !important and more specific selectors

4. **Design and Styling Details**
   - Implementing the quotation mark background image with correct positioning
   - Creating consistent card styles with proper border-radius and padding
   - Managing text opacity for different elements (verified status, testimonial text)
   - Styling profile images with border effects and proper sizing

5. **Performance and Optimization**
   - Adding smooth transitions without affecting performance
   - Using CSS custom properties for maintainable color management
   - Organizing CSS with proper grouping of related properties
   - Ensuring the layout transitions smoothly between breakpoints

### Solutions Implemented

To overcome these challenges, I:
- Used CSS Grid's advanced features like grid-column and grid-row
- Implemented CSS custom properties for consistent theming
- Created separate breakpoints with specific layouts for each screen size
- Added transition properties for smooth layout changes
- Organized CSS with clear comments and logical grouping

### What I learned

I learned how to use CSS Grid to create a responsive layout that would adjust to different screen sizes.

### Continued development

I would like to continue to improve my responsive design skills by working on more complex projects.