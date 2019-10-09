`background-size: cover;`
And what cover does is that whatever the width of the viewport, or the element, it'll always try to fit the element inside of the box.

`background-position: top;`
Because what it does is to ensure that whatever the viewport size is that this top of the image here always stays at the top of the container.

```
background-image: linear-gradient(
        to right bottom,#7ed56fb4
        ,#28b4859d),
        url(../img/hero.jpg);
```

The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line. Its result is an object of the <gradient> data type, which is a special kind of <image>.∏

### `clip-path: polygon(0 0 , 100% 0 , 100% 200px, 0 100%);`

The clip-path CSS property creates a clipping region that sets what part of an element should be shown. Parts that are inside the region are shown, while those outside are hidden.

Polygon is the most flexible of all the available shapes because it allows you to specify any amount of points, a little bit like an SVG path. The provided points are pairs of X and Y coordinates that can be of any unit (eg: pixel or percent-based). Because it’s the most flexible, it’s also the most complex and you’ll probably want to use a tool to define your points.

### position

`position:absolute`

`position:relative`

text-transform:uppercase

### block level elements

Because remember that block elements occupy the entire width that they have available. And more importantly for this case, they create line breaks after and before them. And so that's exactly what we want. So a span element is by default, an inline element. So it's just like text. And so we use the display property.

Display, and display it as a block. transform: translateSo we want this middle of the box to be just herewhere now the beginning of the box is. And the same thing applies to the height. So we want this center here of the box,this horizontal center,we want it to be here where the box now begins. So another way,what we want is to translate this entire box. And it's actually pretty easy to do. We just need to use the transform property in CSS. Transform, and translate. Translate. And now we just need to specify how much wewanna translate on x and on epsilon. And what we want is minus 50% for both. And that's it. And that's because these 50% are now no longerin relation to the parent element,but of the element itself. And so if we say we want minus 50%,it will be shifted half of the width to the left side. And the same for the height. So minus 50% says that it will be shifted50% of the element's height to the top.

### transform: translate vs top and left

You can now use these concepts for other things. Because now you totally understand how this worked.

For the Top and Left properties
So again, just to make everything 100% sure. These 40% and these 50%, they are in relation to the parent element.
So 50% of the parent element is where the text box was located to the left side.

Transform: translate
But, on the transform here, when we translated, this is in relation to the element itself.
And this makes it possible that the element is exactly at the center.

## Animations

it's best to only ever animate two different properties.

One is opacity, which is the one that we're using here,

and the other one is the transform property.

That's what the browsers are optimized for,

for these two properties.

### Animation-timing-functions

`animation`
is the shorthand for a number of animation properties

`animation: moveInRight 1s ease-out;`

### `backface-visibility:hidden`

right before the animation ends you will probably

see a little shake here, okay?

So let's take a close look at the end.

no one really knows actually why this happens, but we, actually, we have a fix for this. So there is something that we can do and what we have to do in this case, is to simply declare the backface-visibility property, backface-visibility, and set it to hidden. So the entire heading-primary element because you see actually this entire element is what moves on this animation. So it's a bit shaky, and its the entire heading-primary element. This backface-visibility property determines if the back part of the element when we transform it is visible or hidden for the user.

### Pseudo-Elements and Pseudo-Classes

Pseudo-Classes:
And pseudo-classes are a special state of a selector. So like when a user hovers an element, or when a checkbox is clicked or if we want to select a last-child,
and many other possibilities. So we use pseudo-classes to style elements under a special condition.

---
How to add padding, heights and widths

        So this button here is right now an inline element
        because it's simply text, but we should display it as an inline block. And this way the box model works on this element as if was just a normal block element, okay? So we should always do this if we want to give some paddings or some heights or width to elements, okay?

---

###  `transform: translateY())` - Moving Up and Down the Y Axis
And we want it to move up so we use a negative value
 and that's because in CSS, the upsilon axis moves from the top to the bottom, so it's like from the top to the bottom. And if you want to move up, we have to go the other way around and so it's negative. So to go up, it's a negative value. So negative, minus three pixels in this case.

 ### `transition: all`
 All we have to do is use the transition property,
 transition, now we have to just specify which properties we want to animate. And if we're not really sure, or if we don't want to write them out, we can simply say all. So in this case, all the properties are enabled to be animated.

 #### `transition: all` and Pseudo-Elements
 The `transition: all` property has to be on the initial state

 ---
 Button click css
 ```
 .btn:link,
.btn:visited {
    text-transform: uppercase;
    text-decoration: none;
    padding: 15px 40px;
    display: inline-block;
    border-radius: 100px;
    transition: all .2s;
}
.btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(0,0,0,.2);
}
.btn:active {
    transform: translateY(-1px);
    box-shadow: 0 5px 10px rgba(0,0,0,.2);    
}
```
---

### `::after` Pseudo Element Requirements
First, in order for an after pseudo-element to actually appear on the page, we need to specify **its content property**. So that's always necessary. It doesn't matter what the content is. It can even be empty like we're gonna do here, but we have to specify it. Otherwise it's not going to appear. And the same thing with the display property. So we have to specify the display property.

### setting  height width using `::after`

So we want to have a height of 100%. And we want to have a width of 100% as well. And this works because the after pseudo-element is basically treated like a child of the button. And so if we say that we want the height to be 100%, that's 100% of the width of the button. And so suppose that the button has 100 pixels of height and 50 pixels of width. And so this after pseudo-element will have the exact same dimensions if we set it to 100%.

---

        That's the trick for fading something out, is going to opacity zero

---

### `animation-fill-mode:backwards`
is that it will automatically apply the styles up to zero percent before the animation starts. So, again, these styles will now be applied before the animation starts simply by using the animation fill mode and set it to backwards.