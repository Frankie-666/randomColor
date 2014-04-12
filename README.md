# Random Color

For generating attractive colors with an element of randomness. [See the demo](https://rawgithub.com/davidmerfield/Random-Color/master/demo/index.html).

```javascript
randomColor() // returns '#F7A7D9'
```

### Options

You can pass an options object to influence the type of color it produces. The options object accepts the following properties:

**Hue** – Possible values are *red, orange, yellow, green, blue, purple, pink*. Also accept a hue value between 0 and 360

**Luminosity** – Possible values are *light, dark, bright, dull*.

**Format** – Possible values are *hsv, rgb, rgbArray, and hex*.
 
{count: 10,distinct: true}     

randomColor({hue: 'green', count: 10, distinct: true});

randomColor({
   count: 10, // returns array of 10 colors...
   hue: 'green', // with green hues...
);

randomColor({
   count: 10, // returns array of 10 colors...
   hue: 'distinct', // with distinct hues...
   luminosity: 'bright' // and bright.
);

randomColor({
   count: 10, // returns array of 10 colors...
   hue: {complements: 'blue'}, // with hues which complement blue
);

Here's an example with an options object. This will produce a random orange color:

```javascript
randomColor({hue: 'orange'}) // returns '#F7A7D9'
```

[See more examples on the demo](https://rawgithub.com/davidmerfield/Random-Color/master/demo/index.html)
