# [Accessibility Fundamentals - Disabilities, Guidelines, and Laws](https://dequeuniversity.com/class/fundamentals)

## Introduction
This module explores the needs of people with disabilities and provides important background information about accessibility guidelines, laws, and rationale.

## Types of Disabilities: Personas
In this section, you will learn about the different types of disabilities as well as what you need to consider for each disability as a web designer, developer, quality assurance professional, or project manager. In addition, there are scenarios presented for some disabilities to aid UX designers in understanding requirements for users with disabilities.

### [Blind](https://dequeuniversity.com/class/fundamentals/personas/blind)
#### 🗣️ What's important
- People with blindness mainly need a website that are accessible for **screenreader** to navigate.
  - The persona in this case use their screenreader to read out their notes from previous sessions & reads out online psychology journals/magazines.
  - Screenreaders read out the text in a website into spoken words, they are often speed up so he users can skim the web pages faster.
- Some basic web considerations:
  - All content must be presented in text or via a text equivalent;
  - Information must not be conveyed by visual attributes alone;
  - All functionality must be available using only the keyboard;
  - The content must use markup with good structure and semantics;
  - All custom controls must have the correct name/label, role, and value, and must change value when appropriate;
  - Users must receive immediate feedback after all actions, via their screen reader. Silence after activating a feature is always bad!
  - Videos require audio descriptions if the video's original audio track does not explain everything that a person who is blind would need to know to understand the video.
  - On mobile devices:
    - All features require a click action.
    - Custom swipe actions on web pages will not work with the screen reader turned on.

### [Low Vision](https://dequeuniversity.com/class/fundamentals/personas/low-vision)
#### 🗣️ What's important
- People with low vision have multiple assistive technology to work with their computer/websites:
  - Zoom software to zoom into content on their screen;
  - Keyboard to control the menu/navigation/controls of the website/computer;
  - Color filters for instance inverting the color scheme or filtering out certain colors or adding more contrast, ...;
    - Some people experience light colors as too bright or could be painfull.
  - Screenreaders can be helpfull for them too, some zoom software has a built in screenreader functionality to combine.
- People with low vision are not a single condition, you have multiple conditions with different degrees:
  - **Blur**: Song 2 😏, faces and text seem blurry, they might only be able to distinguish headings.
  - **Blur with low contrast** everything tends to be in the same brightness and make hard to distinguish outlines/borders and details.
  - **Cataracts** dark gray spots
  - **Diabetic Retinopathy** floating dark spots
  - **Glaucoma** no pheripheral vision, edges are dark and vignetted.
  - **Hemianopia** limiting vision to a smaller area
  - **Macular degeneration** central vision loss / blurryness
  - **Retinal detachment** multiple ways, floaters but also larger dark shadows
- Some basic web considerations:
  - The pinch-to-zoom feature must not be disabled (avoid `<meta name="viewport" content="user-scalable=no">`).
  - All text, borders & other elements must pass contrast guidelines against the background
  - Links, buttons, and controls must have a visible `:focus` state and should have a visible `:hover` state.
    - The default browser `:focus` state is acceptable per the WCAG guidelines, but users with low vision benefit greatly from enhanced CSS `:focus` and `:hover` states.
  - The user interface should provide a clear visual distinction between content and controls.