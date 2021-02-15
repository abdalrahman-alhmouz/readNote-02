# What's the Responsive Web Design ?

Responsive web design is the practice of building a website suitable to work on every device and every screen size .

## Responsive vs. Adaptive 

**So what's the deffirence between them ?**

**Responsive** 
1. generally means to react quickly and positively to any change 
2. With responsive design websites continually and fluidly change based on different factors
 while.
 **adaptive** 
 1. means to be easily modified for a new purpose or situation
 2. adaptive websites are built to a group of preset factors

 *BUT*
 A combination of the two is ideal, providing the perfect formula for functional websites.


Responsive web design is broken down into three main components:
1. flexible layouts
2. media queries
3. flexible media


## 1. Flexible Layouts

 It is the practice of building the layout of a website with a flexible grid.

  AND this is the formula to help identify the proportions of a flexible layout using relative values:

  ### target ÷ context = result

  The flexible layout approach alone isn’t enough. At times the width of a browser viewport may be so small that even scaling the the layout proportionally will create columns that are too small to effectively display content.
  In this event, media queries can be used to help build a better experience.

## 2. Media Queries
 
 Media queries were built as an extension to media types commonly found when targeting and including styles.

 There are 2 ways to use media queries :
 1. using the @media rule inside of an existing style sheet 
 /* @media Rule */
@media all and (max-width: 1024px) {...}

/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}


 2. by linking to a separate style sheet from within the HTML document. // < link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">

## Mobile First

It's one popular technique with using media queries . It includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

 
 **Viewport Height & Width**
 For the best results, and the best looking website, it is recommend that you use the device defaults by applying the device-height and device-width values.

 < meta name="viewport" content="width=device-width">

## 3. Flexible Media

*Flexible Media Demo*

![image](https://css-tricks.com/wp-content/uploads/2012/09/flexible-images.jpg)

# What is "Float"?

Float is a CSS positioning property.
There are four valid values for the float property:  Left and Right , None and Inherit .
it can be used to create entire web layouts.

Float's sister property is **clear**. An element that has the clear property set on it will not move up adjacent to the float like the float desires.

## Techniques for Clearing Floats
 
 1. The Empty Div Method
 2. The Overflow Method
 3. The Easy Clearing Method

 






