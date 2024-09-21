# Web Dev Starter Code

## Overview

This module shifts our focus to web page accessibility, encouraging us to examine different styles that improve usability for a variety of users. The aim of this lab is to align the given webpage with the example webpage while prioritizing accessibility.

## Usage

The webpage can be run using the VSCode plugin "Live Preview" to view it on its development server.

## Accessibility Lab Answers
Semantic HTML
1. The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
    - Pressing the Tab key lets me navigate through all the selectable options, including the audio and comment sections. Pressing Enter takes me to the bottom of the page, while the Up and Down keys allow me to scroll. However, I can’t access the "Show Comments" section, and I have to keep tabbing to loop back to my options.      
2. Can you update the article text to make it easier for screen reader users to navigate?
    - I’ve differentiated the various font sizes by converting them into header tags and organized them into paragraphs for clearer distinction. This structure should help screen readers visualize content flow and makes it easier for users to navigate through the content.
3. The navigation menu part of the site (wrapped in "div class="nav /div") could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.
    - It should use nav tag, which is designed for navigation links.

Color
- The text-to-background contrast ratio is 4.08:1, which fails the WCAG AA and AAA standard for normal text and does not meet the WCAG AAA standard for large text.

The Images
- This can be fixed by adding an alt attribute to each image, which will provide a text description for screen reader users. This ensures that they can understand the content and context of the images.

The Audio Player
1. I provided captions and transcripts for the audio content to ensure accessibility for hearing-impaired users.
2. I added a hyperlink to download the audio file for users with older browsers that don't support HTML audio.

The Forms
1.  I added an aria-label to the input element for screen readers, so it's only accessible to them but not the sighted users. 
2. I added label tags for both the name and comment input elements. This seemed to align them nicely without requiring any additional CSS rule changes.

The Show/Hide Comment Control
- I added a tabindex to make the show/hide comment control button keyboard-accessible and implemented an event listener to detect when the Enter key is pressed, allowing users to activate it. 

The Table
- I added aria table roles to improve accessibility, helping screen readers associate rows and columns effectively. And then, I used the aria-describedby attribute to provide context that clarifies the table's content. 

## Sources and Credits

- aria label: https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-label
- color contrast : https://developer.mozilla.org/en-US/docs/Learn/Accessibility/CSS_and_JavaScript
- tab accessibility: https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML