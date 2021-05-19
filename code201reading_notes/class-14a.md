# Transforms:

- All of these new techniques are made possible by the transform property. The transform property comes in two
  different settings, two-dimensional and three-dimensional. Generally speaking, browser support for the transform 
  property isn’t great, but it is getting better every day.

- The actual syntax for the transform property is quite simple, including the transform property followed by the value. 
  The value specifies the transform type followed by a specific amount inside parentheses.


- Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional
  transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both
  the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of 
  an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then 
  work our way into three-dimensional transforms.

- Perspective In order for three-dimensional transforms to work the elements need a perspective from which to transform. 
  The perspective of an element can be set in two different ways. Using the perspective value within the transform property
  works great for transforming one element from a single, unique perspective.


- Transform Style On occasion three-dimensional transforms will be applied on an element that is nested within a parent element 
  which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space. 
  To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value.

## Transitions & Animations:

- There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, 
  and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

- **Transition Duration** The duration in which a transition takes place is set using the transition-duration property.The value of this
  property can be set using general timing values, including seconds (s) and milliseconds (ms).
 
- **Animations** Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds
  of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where 
  animations pick up where transitions leave off.

- **Animations Keyframes** To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes 
  rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

- **Customizing Animations** Animations also provide the ability to further customize an element’s behavior, including the ability to declare 
  the number of times an animation runs, as well as the direction in which an animation completes.

- **Animation Iteration** By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself 
  numerous times the animation-iteration-count property may be used. Values for the animation-iteration-count property include either an integer
  or the infinite keyword.

### 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS:

1. **Fade in** Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.
2. **Change color** Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then 
   recombining them. 
3. **Grow & Shrink** To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.
4. **Rotate elements** CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. 
5. **Square to circle**
6. **3D shadow**
7. **Swing**
8. **Inset border**
