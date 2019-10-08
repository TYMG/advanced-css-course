
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