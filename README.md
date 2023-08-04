## This is a CodePen that creates a Trinity spinner.

# The HTML file contains the following elements:

* A `div` element with the id `container`. This element will contain the spinner.
* A `svg` element with the viewBox `0 0 100 100`. This element will contain the circle that will create the spinner.
* A `defs` element. This element contains a `filter` element with the id `shadow`. This filter will add a shadow to the circle.
* A `circle` element with the id `spinner`. This element is the circle that will create the spinner.

The CSS file contains the following styles:

* The `div` element is positioned absolutely and is centered in the browser window.
* The `#container` element has a width and height of 200px.
* The `#spinner` element has a stroke-dasharray of 1 98 and a stroke-dashoffset of -105. This will create the animation effect.
* The `#spinner` element has a transform-origin of center. This will ensure that the animation rotates around the center of the circle.
* The `#spinner` element has an animation name of animation, a duration of 1.2 seconds, a timing function of cubic-bezier, and an iteration count of infinite. This will create the animation effect.

The JavaScript file contains the following code:

```
anime({
  targets: '#spinner',
  strokeDasharray: [1, 98],
  strokeDashoffset: -105,
  duration: 1.2,
  easing: 'cubic-bezier',
  loop: true
});
```

This code uses the anime.js library to create the animation effect. The `targets` property specifies the element that will be animated. The `strokeDasharray` property specifies the dasharray of the circle. The `strokeDashoffset` property specifies the dashoffset of the circle. The `duration` property specifies the duration of the animation. The `easing` property specifies the easing function of the animation. The `loop` property specifies whether the animation should loop.