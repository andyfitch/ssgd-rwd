RWD - Stack Similarities, Group Differences
========

In the grand scheme of things, responsive web design (RWD) is still in its infancy, and there are a number of different theories on how to use our HTML & CSS toolkit to best adapt to the plethora of devices ready to (attempt to) render your website how you'd like it to render.

One solution is to declare that:

- Attributes common to all devices are given their own descriptive, stacked classes.
- Device-specific attributes are given a generic class. The attributes within these classes are overridden using media queries.

Key considerations:

- Class names are formatted using the block__element--modifier (BEM) methodology
- Less confusing than previous methodologies
- A more explicit representation of what defines a class
- Promotes OOCSS

This solution is built on the inuit.css framework by Harry Roberts at CSS Wizardry, which is packaged up with hundreds of descriptive helper classes, ready to stack on to your elements. It also uses BEM, which is nice! :)