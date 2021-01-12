# Learn to Code Advanced
# HTML & CSS `*Transforms*`

> The transform property comes in two different settings, two-dimensional and three-dimensional.
> Each of these come with their own individual properties and values.

**Transform Syntax***

> The actual syntax for the transform property is quite simple, including the transform property followed by the value. 
> The value specifies the transform type followed by a specific amount inside parentheses.

*Example*

***Rotate, skew, and scale three different `<div>` elements:***

``` ruby
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

# 2D Scaling Functions: `scale`, `scaleX`, and `scaleY`

![](https://i0.wp.com/lenadesign.org/wp-content/uploads/2020/02/skew.gif?resize=580%2C435&ssl=1)


> With scaling functions, we can increase or decrease the rendered size of an element in the X-dimension (scaleX), Y-dimension (scaleY), or both (scale). Scaling is illustrated below, where the border illustrates the original boundaries of the box, and the + marks its center point.


# 3D transform functions

![](https://gutenberghub.com/wp-content/uploads/2020/01/Screen-Recording-2020-01-18-at-01.38-PM.gif)

> As a web designer, you’re probably well acquainted with working in two dimensions, `X `and `Y`, positioning items horizontally and vertically.
> With a 3D space initialized with perspective, we can now transform elements in three spatial dimensions with the third Z dimension.

***3D transforms use the same transform property used for 2D transforms. If you’re familiar with 2D transforms, you’ll find the basic 3D transform functions similar.***

- `rotateX( angle )`
- `rotateY( angle )`
- `rotateZ( angle )`
- `translateZ( tz )`
- `scaleZ( sz )`

# Perspective
The `perspective` of an element can be set in two different ways. One way includes using the `perspective` value within the `transform` property on individual elements, while the other includes using the `perspective` property on the parent element residing over child elements being transformed.

# Animations
> When multiple transitions are required, the transition property becomes obsolete and the animation property becomes the focus. To set multiple points at which an element should transition, we use the` @keyframes` rule, which includes the animation name, any animation breakpoints, and the properties intended to be animated.

``` ruby
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```

