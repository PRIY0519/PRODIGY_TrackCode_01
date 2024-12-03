# PRODIGY_TrackCode_01
TASK1 :- Create an interactive navigation menu that changes color or style when scrolled or when hovering over a menu item. The navigation menu should have a fixed position and be visible on all pages. Use HTML to structure the menu, CSS to style it, and JavaScript to add interactivity, such as changing the background color or font color of the menu when it is scrolled or when a menu item is hovered over.
**DESCRIPTION OF MY CODE**
**HTML_FILE** (SAVE AS Task.html)
This HTML file represents the structure of a simple webpage with a navigation header, main content section, and footer. Here's a breakdown of its key elements:
**DOCTYPE and Language Declaration:**
<!DOCTYPE html>: Declares the document type as HTML5.
<html lang="en">: Specifies the language of the webpage as English.
**Head Section:**
<title>My Website</title>: Sets the title of the webpage that will appear in the browser tab.
<link rel="stylesheet" href="task1.css">: Links an external CSS file (task1.css) to style the webpage.
**Body Section:**
_Header:_
Contains a <nav> element that holds navigation links (Home, About, Services, and Contact Us).
The header class is used for styling the header element.
_Main Content:_
Includes a welcoming section with a heading, a quote (with a CSS class for styling), and an embedded animated welcome image from an external URL (displayed as a GIF).
The main content section is wrapped inside a <section> element, and there is a div inside it that may be used for further content.
_Footer:_
Contains a copyright notice (&copy; 2024 Priya. Build By PG), showing the year and credits for the website's creation.
_Dark Mode Button:_
The div with the ID dark and the class dark likely serves as a button or toggle for dark mode functionality, though its behavior is not defined in the provided code (requires additional JavaScript or CSS for functionality).
An icon for the moon (<i class="fas fa-moon"></i>) is included to represent the dark mode toggle.
Summary:- 
  This is a basic webpage template that features a header with navigation links, a main content area with a welcome message, an image, and a footer with copyright information. The page includes placeholders for styling (task1.css) and potential dark mode functionality.

**CSS_FILE** (SAVE AS task1.css)
This CSS file styles a webpage with a modern, dark theme, featuring a fixed header, an animated main content section, and responsive navigation. Here's a breakdown of the various styles:
**General Styles:**
html:
The font-size is set to 64.5%, effectively resizing all elements on the page relative to this setting. This may be for responsive design or a custom scaling factor.
body:
The body element is set to take up the entire viewport (width: 100%; height: 100%).
A black background (background: rgb(0, 0, 0)) is applied, giving the page a dark theme.
The text color is set to white (color: #fff) for good contrast on the dark background.
Header Styling:
header:
The header is fixed at the top of the page, staying in place as the user scrolls (position: fixed; top: 0; left: 0;).
It uses a flexbox layout (display: flex; justify-content: space-between; align-items: center) to align its content, such as navigation links, across the header.
Padding of 1rem 9% ensures spacing from the edges, and a drop shadow (filter: drop-shadow(10px)) gives it some depth.
The header has a z-index of 100 to ensure it sits above other page content.
.header:
This is a duplicate of the header styling, likely redundant or used for another element with the same purpose.
Navigation Links:
.navigation a:

Navigation links are styled as inline-block elements with a font size of 1.8rem and white color (color: #fff).
Margins between the links ensure they don't touch each other (margin-left: 4rem).
Hover Effect: When hovered over, links change color to a pinkish shade (rgb(246, 60, 91)) and show a border-bottom with the same color to emphasize interactivity.
Transition: A smooth transition of 0.3s for the color and border effect.
.navigation a.active:

When a navigation link is active, it will also have the pink border and color change, signifying the current page or section.
navigation.active:

This seems to be an attempt to target the active state of the navigation, but there's a typo (navigation should be .navigation or another valid selector).
Main Content Section:
.main-content:

The content section is centered using flexbox (display: flex; justify-content: center; align-items: center;).
It takes up the full height of the viewport minus the header (height: calc(100vh - 80px)), with a column direction for the layout and center-aligned text.
Padding is applied to ensure spacing around the content.
.welcoming-content h1:

The main heading is styled with a large font size (80px) and a pink color (rgb(246, 60, 91)).
A bottom margin is added for spacing (margin-bottom: 20px).
.quote:

The quote text is italicized (font-style: cursive), with a smaller font size (1.6rem) and a white color (color: rgb(255, 255, 255)).
.welcome-image:

The image is centered with a width of 50% and an auto height to maintain aspect ratio.
Border radius gives it rounded corners, and it has a fade-in animation applied that makes it gradually appear on the screen (opacity: 0; animation: fadeIn 2s forwards;).
Animations:
@keyframes fadeIn:
This animation makes the .welcome-image element gradually fade in and move from below (translateY(50px) to translateY(0)), with an opacity change from 0 to 1 over 2 seconds.
@keyframes fadeInContent:
Similar to fadeIn, this animation applies to the header (h1) and paragraph (p), making them fade in and move up from a lower position (translateY(20px) to translateY(0)). This happens over 1 second, with the final opacity being 1.
This CSS file creates a modern, visually appealing webpage with:
Summary:-
A dark theme with white text for high contrast.
Fixed header and responsive navigation with hover effects.
Centered main content with a welcoming message and an animated GIF that fades in.
Smooth animations applied to text and images to improve user experience.
