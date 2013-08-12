A solution for responsive web design - Stack Similarities, Group Differences
========

In the grand scheme of things, responsive web design (RWD) is still in its infancy, and there are a number of different theories on how to use our HTML & CSS toolkit to best adapt to the plethora of devices ready to (attempt to) render your website how you'd like it to render.

A new solution is to give device-agnostic attributes descriptive, stacked classes. Conversely, device-specific attributes exist within two classes; one for dimensions (prefixed with d- for dimensions), and one for appearance and behaviour (prefixed with a- for appearance). The attributes within these classes are overridden using media queries.

Any attributes that remain identical across all devices are given their own helper class.
- These classes are designed for rapid development.
- Stacked together these classes will generate a 'common-denominator' element, which will look identical across all devices.

Any property which varies across multiple devices should be overridden using media queries.
- Avoids describing the ever-growing list of different devices within the class list itself, leaves the differentiation and breakpoint descriptions to the media queries.

Class names are formatted using the block__element--modifier (BEM) methodology
- Less confusing than previous methodologies
- A more explicit representation of what defines a class
- Promotes OOCSS

This solution is built on the inuit.css framework by Harry Roberts at CSS Wizardry, which is packaged up with hundreds of descriptive helper classes, ready to stack on to your elements. It also uses BEM, which is nice! :)