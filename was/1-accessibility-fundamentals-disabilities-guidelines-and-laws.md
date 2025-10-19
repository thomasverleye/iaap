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

### [Color blindness](https://dequeuniversity.com/class/fundamentals/personas/colorblind)
- Color blindness refers to the inability to distinguish between certain kinds of colors, especially colors that are of equal brightness or luminosity, even if the colors themselves appear quite different to people without color-blindness.
- There are several kinds of color blindness and varying in degrees:
  - Red and Green Colorblindness (most common)
    - Deuteranopia and Protanopia are two common sub-types of red-green color-blindness.
  - Blue-yellow color-blindness or Tritanopia
  - Achromatopsia see colors in grayscale
  - Red and Black Colorblindness, though red is visible it becomes for them hard to read on black background in a contrast way.
- Main best practices are to not use color alone for indicating UI but give textual or symbols for indicative explanaition.
- There are no assistive technologies, except maybe some glasses that compensate.

### [Deaf](https://dequeuniversity.com/class/fundamentals/personas/deaf)
- Deaf people do have quite a few assistive tech to help them:
  - Siri or other software to interpret language to text
  - Audio or Video can have captions, especially video needs a transcription. For a deaf and blind person it's even more important as they'll convert the transcript to braille.
- Main web rules:
  - All video needs captions
  - All audio only content must have a transcript
  - Sign language interpretation of videos an be very helpful

### [Deafblind](https://dequeuniversity.com/class/fundamentals/personas/deafblind)
- Deafblind people rely mainly on their braille display, a device that uses a screenreader to get text into raised dots.
- All rules of blindness and deafness apply for them.

### [Motor Disabilities](https://dequeuniversity.com/class/fundamentals/personas/motor)
- Motor disabilities vary in a large range of physical experience:
  - Temporary inability to use a single hand due to an injury;
  - Difficulty using both hands (dexterity disability);
  - All the way to having little to no motor control of your limbs.
  - Lou gehrig's disease (ALS)
- Some people with motor disabilities use following assistive tech:
  - Assistive software along with hardware like an alternative input device or switch.
  - There is no single recommendation for people with motor disabilities.
- Stephen Hawking had a sensor to sense movement in his cheek to interact with his computer screen which had options display so the computer could read out his input.
- Marie-Fance Bru (also ALS or Amyotrophic lateral sclerosis). She uses a sensor on her cheeck to interact with a switch to interact with a custom keyboard in a software program.
- Actor Christopher Reeve has a cervical spinal injury that left him paralyzed from the neck down.
  - Not able to use his legs and hans or torso.
  - He uses an elecrtic wheelchair powered by puff and sip control.
  - Used voice recognition software and other assitive technology to write a book.
- Assistive Technologies Used by People with Motor Disabilities
  - Vertical keyboard with Mouth Stick
  - One-Handed Keyboard
  - Expanded Keyboard with Raised Sections Between Keys
  - Speech recognition (eg dragon)
- Some main considerations on the web:
  - All functionality must be available using only the keyboard.
  - Links, buttons, and controls must have a visible `:focus` state and should have a visible `:hover` state.
  - With session time-outs, warn users before the time expires (e.g. an accessible dialog or alert), and give them the option to extend the session. Ensure the warning itself allows for slow responses. A recommended minimum response time is **2 minutes**.
  - Provide large click targets (links, buttons, controls) for users who have movements that are difficult to control.

### [Speech Disabilities](https://dequeuniversity.com/class/fundamentals/personas/speech)
- Types of Speech Disabilities
  - **Stuttering** is a speech disability that affects the fluency of speech sounds. Involuntarily repeated or prolonged sounds, or sometimes blocked or completely stopped.
  - **Cluttering** is a disability that affects the fluency of speech. Cluttering consists of rapid speech that may be inconsistent in rhythm and lack syntax, or grammar.
  - **Apraxia** is a motor speech disability that occurs when a person has difficulty using muscles for speech production to form sounds of words. It may take a person several attempts to say the correct word.
  - **Dysarthria** is a motor speech disability that occurs due to brain damage. The muscles for speech production are impaired, causing slurred speech, slow speech, mumbling, or a voice that may sound hoarse or breathy.
  - **Speech sound disorders** are generally categorized as articulation disorders or phonemic disorders, that are disorders where certain sounds of speech may be difficult to produces.
  - **Mutism** is the coplete inability to produce a speaking voice.
- Communication options:
  - **Unaided AAC** is the use of nonverbal communication like body language, facial expressions, gestures and sign language.
  - **Aided AAC** vary between electronic and non-electronic tools and person's body. Such as a communication book or board, pen and paper or computers that produces generated voices.
- Main best practice on the web: **Don't depend on voice input**.

### [Cognitive Disabilities](https://dequeuniversity.com/class/fundamentals/personas/cognitive)
- Cognitive disabilities are disabilities in the brain that are a result of congenital conditions that can form through different reasons (Birth, development conditions at young age, traumatic injury, infections, chemical imbalance or other conditions).
- There is no 1 description as there so many kinds and varies in those kinds.
- Web Accessibility for Cognitive Disabilities:
  - **Limited Comprehension** (Hard to understand metaphors, abstractions, slang or idiomatic expressions)
  - **Low Tolerance for Cognitive Overload** (too much things happening at the same time, they need things to be simple)
  - **Limited Problem-Solving Skills** some people may be unable to solve tasks (like CAPTCHA)
  - **Short-Term Memory Loss** some people have a hard time remembering things. So online purchasing procedures or other stuff that could take up some time.
  - **Attention Deficit** for some people it is hard to keep track of your thoughts on websites with too distracting elements like advertisements so they may forget what they wanted to do on the website.
  - **Difficulty Reading** some people are behind with their peers or cannot read at all. It is helpful to provide illustrations or audio. Some people with dyslexia might have a high cognitive function but have a hard time spelling or reading words.
  - **Difficulty Understanding or Using Math** some cannot solve math or have anxiety to solve math.
- Best practices:
  - For lower comprehension:
    - Simplify the interface
    - Simplify the content
    - Keep media short as possible
    - Limit the amount of choices
    - Provide help features
    - Design for ease of use
    - Test the usability of the interface with actual audience
  - For memory loss:
    - Retain information across screens, and within a path.
    - Provide help features.
  - For users with distractibility:
    - Reduce or eliminate distractions (be careful with ads, carousels, intrusive audio, intrusive video, etc.).

### [Reading Disabilities](https://dequeuniversity.com/class/fundamentals/personas/reading)
- See previous part for people with cognitive disabilities and reading.
- **Dyslexia** is a disabilitie where people see letters appearing to be moving around and swap eachother out of place.
- For users with difficulty reading (dyslexia, etc.):
  - Supplement text with illustrations, videos, audio, etc.
  - Avoid the highest level of contrast for text against background (e.g., black on white) BUT be sure to stay within the contrast range that people with low vision need.

### [Seizures](https://dequeuniversity.com/class/fundamentals/personas/seizures)
- Seizures can be caused by a wide range of circumstances including brain injury, dehydration, sleep deprivation, infections, fevers, drug overdoses, drug withdrawals, and even flashing lights.
- Photo-Epileptic Seizures is triggered through people who view flashing or strobe type effects in videos or graphics.
  - Not all epileptical are triggered through lights.
- Best practices for the web: Don't include videos, animations, or transitions with flashing light sequences of **3 times or more per second.**

### [Multiple Disabilities](https://dequeuniversity.com/class/fundamentals/personas/multiple)
- Mainly concider following all other accessibility standards so you can support these people as much as possible.

