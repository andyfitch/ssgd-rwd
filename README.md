ssgd-rwd
========

A solution for responsive web design

In the grand scheme of things, responsive web design (RWD) is still in its infancy, and there are a number of different theories on how to use our HTML & CSS toolkit to best adapt to the plethora of devices ready to (attempt to) render your website how you'd like it to render.

A new solution is to give device-agnostic attributes descriptive, stacked classes. Conversely, device-specific attributes exist within two classes; one for dimensions (prefixed with d- for dimensions), and one for appearance and behaviour (prefixed with a- for appearance). The attributes within these classes are overridden using media queries.

- Any attributes identical constant across all devices are given their own helper class.
* These classes are designed for rapid development.
* Stacked together these classes will generate a 'common-denominator' element, which will look identical across all devices.

- Any property which varies across multiple devices should be overridden using media queries.
* Avoids the need for describing different devices within the class list itself, leaves the differentiation and breakpoint descriptions to the media queries.
* Attributes

- Class names are formatted using the block__element*modifier (BEM) methodology
* Less confusing than previous methodologies
* A more explicit representation of what defines a class
* Promotes OOCSS

- This solution is built on the inuit.css framework, which is ideal for stacking descriptive classes using BEM.