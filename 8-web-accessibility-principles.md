# [Web Accessibility Principles](https://dequeuniversity.com/class/iaap-cpacc/principles/)

> [!NOTE]
> **Learning Goals of this Section**  
> 1. Name the four main principles of web accessibility.
> 2. Describe how each principle is applied to web design and development.

## Perceivable

### Definition
Perceivability is about making the output of web content available through multiple sensory modalities.

### Biological Pathways to Perception
You need to be able to perceive the web through at least one of your biological senses (Sight, Sound, Touch, Taste, Smell) we're only going to focus on **Sight, Sound and Touch** as the others aren't possible or applied in a general way.  

#### Seeing Web Content
Web designer/developer don't (or rather don't) realise their vision isn't as clear as people with less good vision as theirs so they don't take that into account.

**It's important the web is preceivable for people who have lower vision.**

#### Hearing Web Content
People who are (partially) blind rely on their hearing. They can browse web content through hearing and control web applications in an alternative way instead of point and clicking.

**It's fundamental the web is preceivable for people who use screen readers.**

#### Feeling Web Content
People who are (partially) blind and deaf rely on their touch. They can browse web content through braille devices and keyboards.

**For people who are deaf and blind it's important all web content has textual alternative so their braille devices can read it out.**

### Why Perceivability Matters
**If you can't perceive web content, it may as well not exist.**
- Visual info is useless if no digital text alternatives aren't provided if you cannot see.
- Audio content is useless if no digital text alternatives if you cannot hear.

### Making Dynamic Content Perceivable
You can and need to make dynamic content interactable, through the use of **ARIA** ("Accessible Rich Internet Applications"), such as:
- when a tab is "expanded" or "collapsed";
- new content as it is inserted into the DOM;
- error message or a confirmation message;

### Make Sure Users Know What's on the Web Page
Content can't be accessed if users don't know if it is there. You content needs to be availble for Sight, Sound and Touch.  
**Digital text** — whether visible or hidden (using valid accessibility techniques) — is the **most universal method** of accomplishing the broadest perceivability.

## Operable

### Definition
Operability is about making the input methods of web content functionally available to a wide range of input devices.

### Not Everyone Uses a Computer Like You Do
Not everyone can use a mouse or keyboard because of several possible disabilities.

### Everything Has to Work
All content that is interactive should be interactive for everyone, even people who cannot use a mouse and/or keyboard.

### In, Within, Through, and Out
You have to be able to navigate into web components, use the features within them, navigate through them, and navigate out of all of them, no matter what input device you're using.

### Scripting for Device Independence
When you write scripts on the web and overwrite behaviour of standard components OR create new custom ones you need to take all input devices into account.

### Control the Focus
When opening dialogs etc, make sure your focus moves to the correct spot, and when closing those kind of elements, return to the previous focus point.

### Timing
When providing lengthy forms or pages that might need a lot of time for users (even without disabilities). Ensure they have enough of time, even maybe preventing time limits. Prevent that sessions timeout and if needed, make sure you create an accessible notification for it.

### Keyboards: The (almost) Universal Input Device
A lot of users with disabilities use keyboards or devices that are based on how keyboards work. So it's quite often said that if you can **operate** the web content with a keyboard it's almost be operable for everyone. The mouse however is still also important though.

## Understandable

### Definition
Understandability is about making content and interfaces that people can comprehend.

### Understandable content

#### Specify the Language
Use `lang="<language>"`.

#### Simplify the Reading or Vocabulary level
Keep in mind people with reading disorders.

#### Limit or Avoid Terminology or Concepts that are Unfamiliar or Complex
Some people with more generalized cognitive disabilities are unable to understand complex ideas and abstractions.

#### Provide Supplemental Formats
There are some people who cannot read at all, they need alternative content like video, audio, images, ...
Providing content alternatives this extreme might be hard and ain't mandatory. BUT, providing these alternative not only benefits those people. It will also benefit for others as your content becomes easier to comprehend.

### Understandable Interfaces and Interactivity

#### Consistency and Predictability
Make sure your navigation stays the same through all pages. Make sure your form and other controls work as they standarly work in their browser. And when creating a complete custom component with a new kind of interaction, which you need to avoid at all times, provide instructions so user can learn how to use it.

### Assistance: Error Prevention and Correction

#### Provide Instructions, Hints, and Contextual Help

When you need user input, provide:
- instructions on why you need it and what they should do;
- fields with constraints need extra instructions;
  - Required;
  - Read-only or disabled;
  - Data needs to be in certain format;
  - Password strength requirements;
  - Certain length of characters;
  - ...

#### Provide Feedback with Confirmation and Error Messages
Provide success and error messages.

## Robust

### Definition
Robustness is about ensuring compatibility with a broad range of user agents, including assistive technologies.

### Browser compatible
Make sure your website is interpretable for all browsers.

### Use Standard Markup
You can increase robustness by using standard markup and validating it. This is no guarantee for better accessibility, but it will eliminate problems you might get in other user agents.

### Use ARIA (or other means) to Indicate the Name, Role, and Value of Interactive Components
Basically same text as operable. But also that there are a lot of rich elements that have their own role preceivable for users with screenreaders.