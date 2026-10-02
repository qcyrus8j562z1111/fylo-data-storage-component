# Frontend Mentor - Fylo Data Storage Component Solution
 
This is my solution to the Fylo Data Storage Component challenge on Frontend Mentor. This project focused on building a responsive component from provided mobile and desktop designs using HTML and CSS.
 
## Table of Contents
 
- #overview
- #the-challenge
- #screenshot
- #links
- #my-process
- #built-with
- #what-i-learned
- #continued-development
- #ai-collaboration
- #author
 
## Overview
 
### The Challenge
 
Users should be able to:
 
- View the optimal layout for the component depending on their device's screen size
 
### Screenshot
 
./screenshot.jpg
 
### Links
 
- Solution URL: Add Frontend Mentor solution URL after submission
- Live Site URL: Add GitHub Pages URL after deployment
- Repository: https://github.com/qcyrus8j562z1111/fylo-data-storage-component
 
## My Process
 
I approached this project using a mobile-first workflow. I first built the HTML structure for the two main cards and then styled the mobile layout before introducing a media query for larger screens.
 
I also used Git throughout development and made commits at meaningful milestones so the repository shows the progression of the project rather than containing only one final commit.
 
### Built With
 
- Semantic HTML5
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Responsive media queries
- CSS gradients
- CSS pseudo-elements
- Relative and absolute positioning
- Git and GitHub
 
### What I Learned
 
This project gave me more practice deciding when Flexbox should control layout and when positioned elements are more appropriate.
 
One example was the storage progress indicator. The outer element represents the complete storage capacity, while the inner element represents the amount used:
 
```css
.storage-bar-fill {
position: relative;
width: 81.5%;
height: 100%;
background: linear-gradient(
to right,
var(--color-gradient-start),
var(--color-gradient-end)
);
border-radius: 999px;
}
```
 
The `81.5%` width corresponds to 815 GB used out of 1000 GB.
 
I also used a pseudo-element for the small indicator at the end of the progress bar instead of adding another HTML element purely for decoration:
 
```css
.storage-bar-fill::after {
content: "";
position: absolute;
top: 50%;
right: 0.125rem;
width: 0.625rem;
height: 0.625rem;
background-color: white;
border-radius: 50%;
transform: translateY(-50%);
}
```
 
Another important lesson was responsive debugging. A small difference between `.storage` and `.storage-component` prevented my desktop Flexbox rules from applying. Working through that issue reinforced how important it is to inspect selectors and verify which CSS rules the browser is actually applying instead of immediately adding more code.
 
### Continued Development
 
I want to continue improving my ability to translate design files into responsive layouts without relying on fixed dimensions everywhere.
 
I also want to keep developing my understanding of:
 
- Flexbox alignment
- Responsive breakpoint decisions
- Relative and absolute positioning
- CSS pseudo-elements
- Accessible HTML structure
- Debugging responsive layouts with browser developer tools
 
For future projects, I want to continue building mobile-first and testing intermediate viewport sizes rather than focusing only on the supplied mobile and desktop design widths.
 
### AI Collaboration
 
I used Microsoft 365 Copilot as a learning and debugging partner during this project.
 
Rather than generating the entire finished solution at once, I worked through the project section by section. AI assistance was used to discuss HTML structure, explain CSS concepts, reason through responsive layout decisions, and debug problems during development.
 
One useful part of the process was debugging the desktop layout. Some suggested changes did not work as expected, so I reverted to the last working state, tested individual CSS changes, inspected selectors, and identified the problem before continuing. This reinforced the importance of understanding and verifying suggested code rather than copying it without testing.
 
## Author
 
- GitHub: https://github.com/qcyrus8j562z1111
- Frontend Mentor: Add your Frontend Mentor profile URL