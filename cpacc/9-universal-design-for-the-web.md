# [Universal Design for the Web](https://dequeuniversity.com/class/iaap-cpacc/universal-design-for-web/)

Create products and environments that the vast majority of people can use, taking into account our natural physical diversity. It's broader than the concept of accessible design for people with disabilities.

> [!NOTE]
> **Learning Goals of this Section**  
> To prepare for the web accessibility portion of the exam, be sure you can:
> 1. Identify challenges people with disabilities face while using the web.
> 2. Discuss ways in which universal design can be utilized to make web content accessible based on different types of disabilities.


## Images
People with blindness won't be able to see your picture, so provide an alternative text (`alt` attribute).

If you don't a screen reader will possible read out the filename of the image, which often does not explain that much to the end user.

## Color
Some people with low vision cannot distinguish all colors, don't rely on color alone to convey meaning. Always supplement color-code information with text explanations.

## Contrast
Some people with low vision have low contrast in their sight, ensure the contrast of the text against the background is sufficient to allow the text to be read easily.

## Video & Audio
Deaf people cannot hear content with audio and blind people cannot see what happens in video, provide synchronized captions for the deaf, synchronized audio descriptions for the blind, and a text transcript for those who are both deaf and blind.

## Links
Ensure the link text clearly explains the destination or purpose of the link.

## Headings
Use headings to create a properly-structured outline of the page. This outline helps organize the content, and also improves navigation for screen reader users.

## Keyboard Accessibility
Ensure that all functionality is keyboard-accessible, that the tab order is logical, and that the focus indicator is always visible to sighted keyboard users.

## Tables
Associate data cells with header cells to allow screen reader users to navigate effectively within tables.

## Forms
Every form element needs a label, and that label must be associated explicitly with the form element in the markup.

## Dynamic JavaScript
Make dynamic JavaScript accessible by marking up the name, role, state, properties of elements appropriately with ARIA (and changing them dynamically if necessary), and by controlling keyboard focus.

## PDF Documents
To make a PDF document accessible, it must be in "tagged PDF" format, and must be edited for reading order, tab order, and other semantic and structural markup. Also provide an accessible alternative to the PDF document.